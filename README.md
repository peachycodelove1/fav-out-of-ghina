# fav-out-of-ghina
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy Birthday, Ghina!</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background: linear-gradient(to bottom, #783F03, #513314);
            color: #d7b117;
            margin: 0;
            padding: 0;
            text-align: center;
        }
        h2 {
            color: #e2ba18;
        }
        .message {
            background: rgba(128, 0, 32, 0.8);
            padding: 20px;
            margin: 20px auto;
            border-radius: 10px;
            max-width: 600px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.5);
        }
        .photos img {
            margin: 10px;
            border-radius: 10px;
        }
        footer {
            margin-top: 20px;
            color: #d7b117;
            font-size: 0.9em;
        }
        #game {
            margin-top: 30px;
            padding: 20px;
            background: rgba(128, 0, 32, 0.8);
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.5);
        }
        #game input[type="number"], #game button {
            margin: 10px;
            padding: 10px;
            border-radius: 5px;
            border: none;
        }
        #game input[type="number"] {
            width: 80px;
            text-align: center;
        }
        #game button {
            background-color: #e2ba18;
            color: #783F03;
            font-weight: bold;
            cursor: pointer;
        }
        #game button:hover {
            background-color: #d7b117;
        }
        .prize-code {
            color: #ffeb3b;
            font-weight: bold;
            font-size: 1.2em;
            margin-top: 15px;
        }
    </style>
</head>
<body>
    <h1>Happy Birthday, Ghina!</h1>
    <h2>🎉 Wishing You the Best Day Ever! 🎉</h2>
    <div class="message">
        <p>Hey girlyyyy,</p>
        <p>I hope your birthday is just as wonderful as you. Ever since I met you (ELO), you’ve been amazing, lovely, and beautiful—even if you're growing old 🤭.</p>
        <p>Hope me and you stay friends through college and hopefully (if you find someone as great) your wedding!</p>
        <span style="font-size: 12px;">P.S. I left you a game you can play. Once you beat it, I'll give you your 2nd gift until your next birthday.</span>
        <p><strong>With love, Aylin</strong></p>
    </div>

    <h2>🎥 A Special Video for You!</h2>
    <video controls width="400">
        <source src="C:\Users\hello world\Desktop\ghinaa.mp4"										 type="video/mp4">
        Your browser does not support the video tag.
    </video>

    <div class="photos">
        <img src="C:\Users\hello world\Desktop\taylor.jpeg" alt="Photo 1" width="150" height="150" />
        <img src="C:\Users\hello world\Desktop\gogo.jpeg" alt="Photo 2" width="150" height="150" />
        <img src="C:\Users\hello world\Desktop\princess.jpeg" alt="Photo 3" width="150" height="150" />
    </div>

    <!-- Mini-Game Section -->
    <div id="game">
        <h2>🎮 Mini Game: Guess the Number!</h2>
        <p>I'm thinking of a number between 1 and 20. Can you guess it?</p>
        <input type="number" id="guess" placeholder="1-20" min="1" max="20">
        <button onclick="playGame()">Guess</button>
        <p id="game-message"></p>
        <p id="prize-code" class="prize-code"></p>
    </div>

    <footer>
        &copy; 2024 Made with ❤️ by Aylin (the oldest)
    </footer>

   <script>
    // The correct number is always 16
    const correctNumber = 16;

    function playGame() {
        const userGuess = parseInt(document.getElementById('guess').value);
        const prizeCodeElement = document.getElementById('prize-code');

        if (!userGuess || userGuess < 1 || userGuess > 20) {
            alert('❌ Please enter a valid number between 1 and 20.');
        } else if (userGuess === correctNumber) {
            alert(`🎉 Congrats, you guessed it! The number was ${correctNumber}.\n🎁 Code: GHINA2025\nSend this code as pic to Aylin for a prize!`);
            prizeCodeElement.innerHTML = `🎁 Code: <em>GHINA2025</em><br>Send this code to Aylin for a prize!`;
            document.getElementById('guess').disabled = true;
        } else if (userGuess < correctNumber) {
            alert('📉 Too low! Try again.');
        } else {
            alert('📈 Too high! Try again.');
        }
    }
</script>

    </script>
</body>
</html>
