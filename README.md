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
<!DOCTYPE html>
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
    }, 7000);
}
</script>

</body>
</html>







