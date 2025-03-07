<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Шуточный запрос Cookie</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            margin-top: 100px;
        }
    </style>
</head>
<body>

    <h1>Просьба ввести cookie (или что-то похожее, например coo_ie):</h1>
    <input type="text" id="cookieInput" placeholder="Введите coo_ie">
    <button onclick="checkCookie()">Подтвердить</button>

    <p id="response"></p>

    <script>
        function checkCookie() {
            const userInput = document.getElementById('cookieInput').value;
            const response = document.getElementById('response');
            
            if (userInput.toLowerCase() === 'cookie' || userInput.toLowerCase() === 'coo_ie') {
                response.innerText = "Спасибо, cookie принято!";
                response.style.color = "green";
            } else {
                response.innerText = "Это не cookie. Попробуй снова!";
                response.style.color = "red";
            }
        }
    </script>

</body>
</html>
