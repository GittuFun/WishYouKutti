<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy Birthday!</title>
    <style>
        body {
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            background: linear-gradient(135deg, #ff9a9e, #fad0c4);
            font-family: 'Arial', sans-serif;
            color: #333;
            text-align: center;
        }
        h1 {
            font-size: 3em;
            margin: 0;
        }
        p {
            font-size: 1.5em;
            margin: 10px 0;
        }
        button {
            padding: 10px 20px;
            font-size: 1em;
            background-color: #ff6b6b;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background 0.3s;
        }
        button:hover {
            background-color: #ff4d4d;
        }
        .balloons {
            position: fixed;
            top: 0;
            left: 50%;
            transform: translateX(-50%);
            animation: float 5s infinite;
        }
        @keyframes float {
            0% { transform: translate(-50%, -10%); }
            50% { transform: translate(-50%, 0); }
            100% { transform: translate(-50%, -10%); }
        }
    </style>
</head>
<body>
    <div class="balloons">
        🎈🎈🎈
    </div>
    <h1>🎉 Happy Birthday! 🎉</h1>
    <p>Wishing you a day filled with love, joy, and amazing surprises!</p>
    <button onclick="revealMessage()">Click for a Surprise!</button>
    <p id="message" style="display:none;">You're one of a kind! Have the best birthday ever! 🎂🎁</p>

    <script>
        function revealMessage() {
            document.getElementById('message').style.display = 'block';
        }
    </script>
</body>
</html>
