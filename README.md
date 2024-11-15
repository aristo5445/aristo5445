<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Beautiful Dynamic Website</title>
    <style>
        /* Resetting default styling */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: Arial, sans-serif;
        }

        body {
            overflow-x: hidden;
            background-color: #f3f3f3;
        }

        /* Navbar styling */
        nav {
            background: rgba(0, 0, 0, 0.7);
            color: #fff;
            padding: 10px 20px;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
        }

        nav a {
            color: #fff;
            text-decoration: none;
            margin: 0 15px;
            font-weight: bold;
        }

        /* Hero section */
        .hero {
            height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            background-image: url('https://via.placeholder.com/1920x1080'); /* Replace with your image */
            background-size: cover;
            background-attachment: fixed;
            color: white;
            text-align: center;
        }

        .hero h1 {
            font-size: 3rem;
            animation: float 3s ease-in-out infinite;
        }

        /* Floating animation */
        @keyframes float {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-20px); }
        }

        /* Parallax scrolling effect */
        .parallax {
            height: 50vh;
            background-image: url('https://via.placeholder.com/1920x1080'); /* Replace with your image */
            background-attachment: fixed;
            background-size: cover;
            background-position: center;
        }

        /* Content sections */
        .content {
            padding: 80px 20px;
            text-align: center;
        }

        .content h2 {
            font-size: 2.5rem;
            margin-bottom: 20px;
        }

        .content p {
            font-size: 1.2rem;
            color: #333;
            line-height: 1.6;
            max-width: 800px;
            margin: auto;
        }

        /* Smooth scrolling effect */
        html {
            scroll-behavior: smooth;
        }

        /* Floating circles for dynamic movement */
        .circle {
            position: absolute;
            border-radius: 50%;
            opacity: 0.7;
            animation: move 10s infinite alternate ease-in-out;
        }

        .circle-small {
            width: 100px;
            height: 100px;
            background-color: rgba(255, 69, 0, 0.3);
            top: 50%;
            left: 20%;
        }

        .circle-large {
            width: 200px;
            height: 200px;
            background-color: rgba(65, 105, 225, 0.3);
            top: 10%;
            right: 15%;
        }

        /* Circle movement */
        @keyframes move {
            0% { transform: translateY(0px) translateX(0px); }
            100% { transform: translateY(-30px) translateX(30px); }
        }
    </style>
</head>
<body>

