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
            background-color: #e0f7fa; /* Light aqua blue background */
            color: #00796b; /* Darker teal text color */
            padding: 0; /* Remove default padding */
            margin: 0; /* Remove default margin */
        }
        /* Button styling for navigation */
        .nav-button {
            background-color: #00796b; /* Lighter teal */
            color: white;
            text-align: center;
            text-decoration: none;
            padding: 10px 20px;
            margin: 0 5px;
            border-radius: 8px;
            font-weight: bold;
            display: inline-block; /* Make buttons inline with margin */
            transition: background 0.3s ease;
            cursor: pointer; /* Change cursor to pointer */
            border: none; /* Remove default button border */
        }
        .nav-button:hover {
            background-color: #004d40; /* Darker teal on hover */
        }
        /* Sections with simplified styling */
        .section1, .section2 {
            border: 2px solid #004d40; /* Dark teal border */
            background-color: #b2dfdb; /* Light teal background */
            padding: 20px;
            margin-bottom: 20px;
            border-radius: 8px;
        }
        button {
            background: linear-gradient(45deg, #00acc1, #00796b); /* Aqua blue gradient */
            border: none;
            color: white;
            padding: 10px 20px;
            font-size: 16px;
            cursor: pointer;
            border-radius: 8px;
            transition: background 0.3s ease, transform 0.3s ease;
        }
        button:hover {
            background: linear-gradient(45deg, #00796b, #004d40); /* Darker gradient on hover */
            transform: scale(1.05); /* Slight zoom effect */
        }
        a {
            color: #004d40; /* Dark teal */
            text-decoration: none;
            font-weight: bold;
        }
        a:hover {
            color: #00796b; /* Lighter teal */
            text-decoration: underline;
        }
    </style>
</head>
<body>
    <!-- Navigation buttons -->
    <h2> Sub Menu: Math and its History </h2>
<div style="display: flex; justify-content: center; gap: 20px; padding: 20px;">
  <div style="text-align: center;">
     <a href="notebook1" style="text-decoration: none;">
        <button style="background-color: #4CAF50; color: white; border: none; padding: 15px 30px; font-size: 16px; border-radius: 8px; cursor: pointer;">
           Basic Addition Calculator
        </button>
     </a>
  </div>


  <div style="text-align: center;">
     <a href="notebook2" style="text-decoration: none;">
        <button style="background-color: #2196F3; color: white; border: none; padding: 15px 30px; font-size: 16px; border-radius: 8px; cursor: pointer;">
           Math Jokes; JS Shell
        </button>
     </a>
  </div>


  <div style="text-align: center;">
     <a href="notebook3" style="text-decoration: none;">
        <button style="background-color: #f44336; color: white; border: none; padding: 15px 30px; font-size: 16px; border-radius: 8px; cursor: pointer;">
           Math's History
        </button>
     </a>
  </div>
</div>


    <!-- First Section -->
    <div class="section1">
        <p>The stickbug meme, known as "Get Stick Bugged LOL," is a playful way to bait people into watching a dancing stickbug. It's a fun and harmless prank that has become quite popular online!</p>
        <button onclick="window.location.href='https://www.youtube.com/watch?v=fC7oUOUEEi4'">NOT a stickbug</button>
    </div>

    <!-- Combined Section -->
    <div class="section2">
        <p><strong>Funny Videos:</strong></p>
        <a href="https://www.youtube.com/watch?v=-xqEABqaEuo">Elijah Wood's Interview</a> | 
        <a href="https://www.youtube.com/watch?v=dQw4w9WgXcQ">Rick Roll</a>
        
        <p>Online pranks are everywhere, and two of the funniest are the Rickroll and the Elijah Wood prank interview. The Rickroll tricks people into watching a video they didn't mean to, while the Elijah Wood interview is a hilarious fake conversation. These pranks are super entertaining and always get a laugh out of me!</p>
    </div>
</body>
</html>

    <!-- Navigation buttons -->
    <h2> Sub Menu: Games+Calculator </h2>
<div style="display: flex; justify-content: center; gap: 20px; padding: 20px;">
  <div style="text-align: center;">
     <a href="cookie" style="text-decoration: none;">
        <button styl++e="background-color: #4CAF50; color: white; border: none; padding: 15px 30px; font-size: 16px; border-radius: 8px; cursor: pointer;">
           Cookie Clicker
        </button>
     </a>
  </div>


  <div style="text-align: center;">
     <a href="snake" style="text-decoration: none;">
        <button style="background-color: #2196F3; color: white; border: none; padding: 15px 30px; font-size: 16px; border-radius: 8px; cursor: pointer;">
           Snake Game
        </button>
     </a>
  </div>


  <div style="text-align: center;">
     <a href="calc" style="text-decoration: none;">
        <button style="background-color: #f44336; color: white; border: none; padding: 15px 30px; font-size: 16px; border-radius: 8px; cursor: pointer;">
           Binary Calculator
        </button>
     </a>
  </div>
</div>





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
<script src="https://utteranc.es/client.js"
        repo="Mom5MoreMins/aranya_student_2025"
        issue-term="pathname"
        theme="github-dark"
        crossorigin="anonymous"
        async>
    </script>
</body>
