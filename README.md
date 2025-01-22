<!DOCTYPE html>
<html lang="pt">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Galeria de Vídeos</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #111;
            color: white;
        }
        .video-container {
            width: 80%;
            margin: auto;
        }
        iframe {
            width: 100%;
            height: 400px;
            border: none;
        }
        .thumbnails {
            display: flex;
            justify-content: center;
            gap: 10px;
            margin-top: 20px;
        }
        .thumbnails img {
            width: 150px;
            cursor: pointer;
            border-radius: 5px;
        }
    </style>
</head>
<body>
    <h1>Galeria de Vídeos</h1>
    <div class="video-container">
        <iframe id="main-video" src="https://www.youtube.com/embed/dQw4w9WgXcQ" allowfullscreen></iframe>
    </div>
    <div class="thumbnails">
        <img src="https://img.youtube.com/vi/dQw4w9WgXcQ/0.jpg" onclick="changeVideo('dQw4w9WgXcQ')">
        <img src="https://img.youtube.com/vi/3JZ_D3ELwOQ/0.jpg" onclick="changeVideo('3JZ_D3ELwOQ')">
        <img src="https://img.youtube.com/vi/tgbNymZ7vqY/0.jpg" onclick="changeVideo('tgbNymZ7vqY')">
    </div>
    <script>
        function changeVideo(videoId) {
            document.getElementById('main-video').src = "https://www.youtube.com/embed/" + videoId;
        }
    </script>
</body>
</html>
