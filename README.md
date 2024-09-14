<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Página Divertida</title>
    <style>
        body {
            background-color: #00FF00; /* Verde fosforescente */
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }

        h1 {
            font-size: 48px;
            font-family: Arial, sans-serif;
            color: white;
            transition: color 0.5s;
        }

        .rainbow {
            animation: rainbow 1s infinite;
        }

        @keyframes rainbow {
            0% { color: red; }
            16% { color: orange; }
            33% { color: yellow; }
            50% { color: green; }
            66% { color: blue; }
            83% { color: indigo; }
            100% { color: violet; }
        }
    </style>
</head>
<body>

    <h1 id="texto">Ricardo es gey</h1>

    <script>
        const texto = document.getElementById("texto");

        texto.addEventListener("click", function() {
            texto.classList.toggle("rainbow");
        });
    </script>

</body>
</html>