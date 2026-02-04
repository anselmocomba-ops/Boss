<!DOCTYPE html>
<html lang="pt">
<head>
    <meta charset="UTF-8">
    <title>Curiosidades de Futebol</title>

    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #0b6623;
            color: white;
            text-align: center;
            padding: 40px;
        }

        .caixa {
            background-color: #ffffff;
            color: #000;
            padding: 20px;
            border-radius: 10px;
            max-width: 500px;
            margin: auto;
        }

        button {
            margin-top: 20px;
            padding: 10px 20px;
            font-size: 16px;
            cursor: pointer;
            border: none;
            border-radius: 5px;
            background-color: #0b6623;
            color: white;
        }

        button:hover {
            background-color: #09541c;
        }
    </style>
</head>
<body>

    <h1>⚽ Curiosidades de Futebol</h1>

    <div class="caixa">
        <p id="curiosidade">
            Clique no botão para ver uma curiosidade de futebol!
        </p>

        <button onclick="mostrarCuriosidade()">Nova curiosidade</button>
    </div>

    <script>
        const curiosidades = [
            "O futebol nasceu oficialmente na Inglaterra em 1863.",
            "Pelé é o único jogador a vencer 3 Copas do Mundo.",
            "O maior estádio do mundo é o Rungrado 1º de Maio, na Coreia do Norte.",
            "Um jogo de futebol tem 90 minutos, mas a bola fica em jogo apenas cerca de 60 minutos.",
            "Cristiano Ronaldo já marcou mais de 850 gols na carreira.",
            "O cartão amarelo e vermelho surgiram na Copa do Mundo de 1970.",
            "O Brasil é a seleção com mais títulos da Copa do Mundo."
        ];

        function mostrarCuriosidade() {
            const numero = Math.floor(Math.random() * curiosidades.length);
            document.getElementById("curiosidade").innerText = curiosidades[numero];
        }
    </script>

</body>
</html>

