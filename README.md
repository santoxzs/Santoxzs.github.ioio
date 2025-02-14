<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dias Amando Você 🤍</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #2e0044; /* Roxo escuro */
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            color: white;
        }
        .container {
            text-align: center;
            background-color: rgba(255, 255, 255, 0.9); /* Fundo branco levemente transparente */
            padding: 20px;
            border-radius: 15px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
            width: 90%;
            max-width: 500px;
        }
        .image-container img {
            width: 100%;
            max-width: 300px;
            border-radius: 10px;
            margin-bottom: 20px;
        }
        .content {
            background-color: #fff;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }
        h1 {
            font-size: 2.5rem;
            color: #e74c3c;
            text-shadow: 2px 2px 5px rgba(255, 255, 255, 0.5);
        }
        .countdown {
            font-size: 2rem;
            margin-top: 20px;
            color: #2c3e50;
        }
        p {
            font-size: 1.5rem;
            color: #e74c3c;
            margin-top: 20px;
            text-shadow: 1px 1px 3px rgba(255, 255, 255, 0.5);
        }
        .hearts {
            font-size: 2rem;
            color: red;
            margin-top: 20px;
        }
        .sparkle {
            font-size: 2rem;
            color: #ffd700;
        }
    </style>
</head>
<body>

<div class="container">
    <div class="image-container">
        <img src="https://github.com/santoxzs/Amor.html/blob/main/IMG-20241203-WA0007.jpg?raw=true" alt="Imagem do casal">
    </div>
    <div class="content">
        <h1>Dias Amando Você 🤍</h1>
        <div class="countdown" id="countdown"></div>
        <p>Você é tudo para mim, minha mulher da minha vida, eu te amarei para sempre, meu amor 🥺✨️</p>
        <div class="hearts">❤️🤍</div>
        <div class="sparkle">✨️</div>
    </div>
</div>

<script>
    const startDate = new Date("September 20, 2024 00:00:00").getTime();

    function updateCountdown() {
        const now = new Date().getTime();
        const timeDiff = now - startDate;

        const days = Math.floor(timeDiff / (1000 * 60 * 60 * 24));
        const hours = Math.floor((timeDiff % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
        const minutes = Math.floor((timeDiff % (1000 * 60 * 60)) / (1000 * 60));
        const seconds = Math.floor((timeDiff % (1000 * 60)) / 1000);

        document.getElementById("countdown").innerHTML = `${days} dias, ${hours} horas, ${minutes} minutos e ${seconds} segundos`;
    }

    setInterval(updateCountdown, 1000);
</script>

</body>
</html>
