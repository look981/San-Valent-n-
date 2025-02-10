# San-Valent-n-
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>San Valentín ❤️</title>
    <style>
        body {
            text-align: center;
            font-family: 'Arial', sans-serif;
            background-color: #ffe6e6;
            color: #ff4d4d;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }
        h1 {
            font-size: 28px;
        }
        .buttons {
            margin-top: 20px;
            position: relative;
        }
        button {
            font-size: 20px;
            padding: 10px 20px;
            margin: 10px;
            border: none;
            cursor: pointer;
            border-radius: 5px;
        }
        #yes {
            background-color: #ff4d4d;
            color: white;
        }
        #no {
            background-color: #999;
            color: white;
            position: absolute;
        }
    </style>
</head>
<body>

    <h1>Yuleimy, ¿quieres ser mi San Valentín? ❤️</h1>
    
    <div class="buttons">
        <button id="yes" onclick="yesClick()">Sí 💖</button>
        <button id="no" onmouseover="moveNo()">No 😢</button>
    </div>

    <script>
        function yesClick() {
            alert("¡Sabía que dirías que sí! 💕🥰");
        }

        function moveNo() {
            let x = Math.random() * window.innerWidth * 0.8;
            let y = Math.random() * window.innerHeight * 0.8;
            document.getElementById("no").style.left = x + "px";
            document.getElementById("no").style.top = y + "px";
        }
    </script>

</body>
</html>
