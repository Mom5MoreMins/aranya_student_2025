---
layout: base
title: Aranya Home
description: Home Page
hide: false
---
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f0f0f0; /* Light gray background */
            color: #333; /* Darker text color */
            padding: 20px;
        }
        /* First div: Bold purple border, fun gradient background */
        .div1 {
            border: 4px solid #8a2be2; /* BlueViolet */
            background: linear-gradient(135deg, #f3e5ab, #f7a1a1); /* Soft yellow to pink gradient */
            padding: 20px;
            margin-bottom: 20px;
            border-radius: 15px;
            text-align: center;
        }
        /* Button: Cool gradient background, rounded corners, and hover effect */
        button {
            background: linear-gradient(45deg, #6a5acd, #00ced1); /* SlateBlue to DarkTurquoise gradient */
            border: none;
            color: white;
            padding: 10px 20px;
            font-size: 16px;
            cursor: pointer;
            border-radius: 10px;
            transition: background 0.3s ease, transform 0.3s ease;
        }
        button:hover {
            background: linear-gradient(45deg, #483d8b, #20b2aa); /* Darker shades on hover */
            transform: scale(1.1); /* Slight zoom effect */
        }
        /* Second div: Green border, playful font */
        .div2 {
            border: 3px dashed #32cd32; /* Lime green */
            background-color: #f5fffa; /* Mint cream background */
            padding: 10px;
            margin-bottom: 20px;
            border-radius: 10px;
            font-style: italic; /* Makes it a bit playful */
        }
        /* Third div: Blue border with a fun box shadow */
        .div3 {
            border: 3px dotted #1e90ff; /* Dodger blue */
            background-color: #e6f7ff; /* Light blue background */
            padding: 10px;
            box-shadow: 5px 5px 15px rgba(0, 0, 255, 0.2);
            border-radius: 10px;
        }
        /* Adding some hover effects to links */
        a {
            color: #ff4500; /* Orange red */
            text-decoration: none;
            font-weight: bold;
        }
        a:hover {
            color: #ff6347; /* Tomato red */
            text-decoration: underline;
        }
    </style>
</head>
<body>
    <!-- First Section in the first div with unique styling -->
    <div class="div1">
        <p>The stickbug meme, known as "Get Stick Bugged LOL," is a playful way to bait people into watching a dancing stickbug. It's a fun and harmless prank that has become quite popular online!</p>
        <button onclick="window.location.href='https://www.youtube.com/watch?v=fC7oUOUEEi4'">NOT a stickbug</button>
    </div>

    <!-- Second Section with fun styles and link titles updated -->
    <div class="div2">
        <p><strong>Funny Videos:</strong></p>
        <a href="https://www.youtube.com/watch?v=IfhMILe8C84">Elijah Wood's Interview</a> | 
        <a href="https://www.youtube.com/watch?v=dQw4w9WgXcQ">Rick Roll</a>
    </div>

    <!-- Another styled div with a paragraph -->
    <div class="div3">
        <p>Online pranks are everywhere, and two of the funniest are the Rickroll and the Elijah Wood prank interview. The Rickroll tricks people into watching a video they didn't mean to, while the Elijah Wood interview is a hilarious fake conversation. These pranks are super entertaining and always get a laugh out of me!</p>
    </div>
</body>
</html>




<!-- marioooooo -->
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mario Running</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            overflow-x: hidden;
            position: relative;
        }
        .mario-gif {
            position: fixed;
            bottom: 0;
            left: -400px; /* Start off-screen */
            height: 100px; /* Adjust based on the GIF size */
            animation: moveRight 5s linear infinite;
        }
        @keyframes moveRight {
            from {
                left: -200px; /* Start off-screen */
            }
            to {
                left: 100vw; /* Move across the viewport width */
            }
        }
    </style>
</head>
<body>
    <img src="https://media.tenor.com/UkvleU1dQK4AAAAi/2d-mario-running.gif" alt="Mario Running" class="mario-gif">
    <a href="secretpage.html" target="_blank">
    <img src="https://media.tenor.com/UkvleU1dQK4AAAAi/2d-mario-running.gif" alt="Mario Running" class="mario-gif">
</a>
</body>
