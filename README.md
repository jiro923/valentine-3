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
        }
        h1 {
            font-family: 'Great Vibes', cursive;
            font-size: 3em;
            margin-top: 50px;
        }
        .message {
            font-size: 1.5em;
            margin: 20px;
        }
        .lily-image {
            width: 80%;
            max-width: 300px;
            height: auto;
            margin: 20px;
        }
        .button-container {
            display: flex;
            justify-content: center;
            margin: 20px;
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
            margin: 0 10px;
            transition: background-color 0.3s;
        }
        .button:hover {
            background-color: #FF6347; /* Tomato */
        }
        .footer {
            margin-top: 50px;
            font-size: 1em;
        }
    </style>
</head>
<body>

    <h1>Will You Be My Valentine?</h1>
    <div class="message">
        <p>Hey Babyy :3</p>
    </div>
    
    <img src="https://www.google.com/search?sca_esv=171dd60bbbb03aa4&rlz=1C1GCEA_enPH1087PH1087&sxsrf=AHTn8zptjfCEMWVkQgbiUpMKcn-pOsc1uw:1738208949591&q=lilies+flower&udm=2&fbs=ABzOT_CWdhQLP1FcmU5B0fn3xuWpA-dk4wpBWOGsoR7DG5zJBpwxALD7bRaeOIZxqOFEngxxsUnG07Fj19ytIn9fWqb4sDjxelNUNq0MnGNTvDqYWgEUkp0YHdVxbWr4arEYI0A-9T3hEf7j8afo8Qqr0ahVX5ht8_5rn3axFrf3YrgOB4kmVELVOP6cKIX0bdzQxUrJhHIHagr-1t5vbFY8LmR9ZIukOg&sa=X&ved=2ahUKEwibifH3xJyLAxUW1TQHHRh4DBIQtKgLegQIHRAB&biw=1451&bih=1057&dpr=0.9#imgrc=1-D74lWzqdzRbM&imgdii=6kWaRnvSdhh8yM"> <!-- Valid image URL -->

    <div>
        <audio controls>
            <source src="https://open.spotify.com/track/3eBHh35RljNlNtM3KhKhmM?si=488bc4dc3cb6447b" type="audio/mpeg"> <!-- Valid audio URL -->
            Your browser does not support the audio element.
        </audio>
    </div>

    <div class="button-container">
        <a href="#" class="button" id="yesButton">Yes!</a>
        <a href="#" class="button" id="noButton" onclick="moveNoButton(event)">No!</a>
    </div>

    <div class="footer">
        <p>"Love is not about how many days, months, or years you have been together. Love is about how much you love each other every single day."</p>
    </div>

    <script>
        function moveNoButton(event) {
            event.preventDefault(); // Prevent the default link behavior
            const noButton = document.getElementById('noButton');
            // Move the button to a random position on the screen
            const randomX = Math.floor(Math.random() * (window.innerWidth - 150)); // 150 is the button width
            const randomY = Math.floor(Math.random() * (window.innerHeight - 50)); // 50 is the button height
            noButton.style.position = 'absolute';
            noButton.style.left = randomX + 'px';
            noButton.style.top = randomY + 'px';
        }
    </script>

</body>
</html>
