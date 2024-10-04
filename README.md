<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Simple Clicker Game</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #f4f4f4;
            padding: 50px;
        }
        #hamster {
            width: 150px;
            cursor: pointer;
        }
        #score {
            font-size: 24px;
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <h1>Hamster Clicker Game</h1>
    <p>Click on the hamster to gain points!</p>
    <img id="hamster" src="https://example.com/hamster.png" alt="Hamster">
    <p id="score">Score: 0</p>

    <script>
        let score = 0;
        const hamster = document.getElementById("hamster");
        const scoreDisplay = document.getElementById("score");

        hamster.addEventListener("click", () => {
            score++;
            scoreDisplay.textContent = "Score: " + score;
        });
    </script>
</body>
</html>
