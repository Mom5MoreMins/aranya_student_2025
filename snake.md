<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Simple Snake Game</title>
    <style>
        canvas {
            border: 1px solid black;
        }
        #rules {
            margin-top: 20px;
        }
    </style>
</head>
<body>

<h1>Simple Snake Game</h1>
<canvas id="gameCanvas" width="400" height="400"></canvas>

<div id="rules">
    <h2>Rules:</h2>
    <ul>
        <li>Use the arrow keys or WASD to control the snake.</li>
        <li>Don't hit the walls!</li>
        <li>The snake doesn't grow; the goal is to eat as many apples as possible without crashing.</li>
    </ul>
</div>

<script>
    const canvas = document.getElementById('gameCanvas');
    const ctx = canvas.getContext('2d');
    const grid = 20;
    let x, y, dx, dy;
    let appleX, appleY;
    let score;
    const speed = 100; // Speed of the game loop in milliseconds

    function resetGame() {
        x = 0; // Start position of the snake
        y = 0;
        dx = grid;
        dy = 0;
        appleX = Math.floor(Math.random() * (canvas.width / grid)) * grid;
        appleY = Math.floor(Math.random() * (canvas.height / grid)) * grid;
        score = 0;
    }

    function draw() {
        ctx.clearRect(0, 0, canvas.width, canvas.height);

        // Draw the apple
        ctx.fillStyle = 'red';
        ctx.fillRect(appleX, appleY, grid, grid);

        // Draw the snake
        ctx.fillStyle = 'green';
        ctx.fillRect(x, y, grid, grid);

        // Move the snake
        x += dx;
        y += dy;

        // Check for wall collisions
        if (x < 0 || x >= canvas.width || y < 0 || y >= canvas.height) {
            alert('Game Over! You hit the wall.');
            resetGame();
        }

        // Check if the snake has eaten the apple
        if (x === appleX && y === appleY) {
            score++;
            appleX = Math.floor(Math.random() * (canvas.width / grid)) * grid;
            appleY = Math.floor(Math.random() * (canvas.height / grid)) * grid;
        }
    }

    function changeDirection(event) {
        switch (event.key) {
            case 'ArrowUp':
            case 'w':
                if (dy === 0) {
                    dx = 0;
                    dy = -grid;
                }
                break;
            case 'ArrowDown':
            case 's':
                if (dy === 0) {
                    dx = 0;
                    dy = grid;
                }
                break;
            case 'ArrowLeft':
            case 'a':
                if (dx === 0) {
                    dx = -grid;
                    dy = 0;
                }
                break;
            case 'ArrowRight':
            case 'd':
                if (dx === 0) {
                    dx = grid;
                    dy = 0;
                }
                break;
        }
    }

    document.addEventListener('keydown', changeDirection);

    // Initialize the game
    resetGame();

    // Set up the game loop
    setInterval(draw, speed);
</script>

</body>
</html>
