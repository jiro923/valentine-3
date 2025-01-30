<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Will You Be My Valentine?</title>
    <link href="https://fonts.googleapis.com/css2?family=Great+Vibes&display=swap" rel="stylesheet">
    <style>
        body {
            background-color: #8B0000; /* Dark Red */
            color: white;
            font-family: Arial, sans-serif;
            text-align: center;
            margin: 0;
            padding: 0;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            height: 100vh;
        }
        h1 {
            font-family: 'Great Vibes', cursive;
            font-size: 3em;
            margin: 20px;
        }
        .message {
            font-size: 1.5em;
            margin: 10px;
        }
        .button-container {
            display: flex;
            justify-content: center;
            gap: 20px;
            flex-wrap: wrap;
            position: relative;
        }
        .button {
            background-color: #B22222; /* Firebrick */
            color: white;
            padding: 15px 30px;
            border: none;
            border-radius: 5px;
            font-size: 1.2em;
            cursor: pointer;
            text-decoration: none;
            transition: background-color 0.3s;
            position: relative;
        }
        .button:hover {
            background-color: #FF6347; /* Tomato */
        }
        .footer {
            margin-top: 30px;
            font-size: 1em;
        }
    </style>
</head>
<body>

    <h1>Will You Be My Valentine?</h1>
    <div class="message">
        <p>Hey Babyy :3</p>
    </div>

    <audio id="valentineSong" src="https://docs.google.com/uc?export=download&id=1xqjwLtFFrFHiZ_a_nD0zV9hCPQyLJTXw"></audio>

    <div class="button-container">
        <button class="button" id="yesButton" onclick="playSong()">Yes!</button>
        <button class="button" id="noButton" onclick="moveNoButton(event)">No!</button>
    </div>

    <div class="footer">
      
    </div>

    <script>
        function playSong() {
            const song = document.getElementById("valentineSong");
            song.play();
            alert("Yay! Can't wait to spend Valentine's with you ❤️");
        }

        function moveNoButton(event) {
            event.preventDefault();
            const noButton = document.getElementById('noButton');
            const randomX = Math.random() * (window.innerWidth - 200);
            const randomY = Math.random() * (window.innerHeight - 100);
            noButton.style.position = 'absolute';
            noButton.style.left = `${randomX}px`;
            noButton.style.top = `${randomY}px`;
        }
    </script>

</body>
</html>
