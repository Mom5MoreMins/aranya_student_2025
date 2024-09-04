---
layout: base
title: Student Home 
description: Home Page
hide: true
---

Aranyas Page

<!DOCTYPE html>
<html lang="en">
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
</html> 
