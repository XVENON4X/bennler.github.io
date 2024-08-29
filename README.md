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
            background-color: #007bff;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            margin: 10px;
        }
        .button:hover {
            background-color: #0056b3;
        }
    </style>
</head>
<body>

<button class="button" onclick="window.location.href='https://whatsmyname.app/'">Wysz. po nicku</button>
<button class="button" onclick="window.location.href='https://facecheck.id'">Wysz. po twarzy</button>
<button class="button" onclick="window.location.href='https://jimpl.com'">Inf. ze zdj.</button>
<button class="button" onclick="window.location.href='https://grabify.link'">Zbieraczka z linku</button>
<button class="button" onclick="openAll()">Otwórz wszystkie</button>

<script>
function openAll() {
    window.open('https://whatsmyname.app/', '_blank');
    window.open('https://facecheck.id', '_blank');
    window.open('https://jimpl.com', '_blank');
    window.open('https://grabify.link', '_blank');
}
</script>

</body>
</html>



