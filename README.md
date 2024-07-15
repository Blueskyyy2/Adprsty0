<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Website Pribadi</title>
    <style>
        body {
            background-color: #00CED1; /* Warna biru laut */
            background-image: url('wallpaper_laut.jpg'); /* Ganti dengan URL wallpaper laut yang Anda miliki */
            background-size: cover;
            color: white;
            font-family: Arial, sans-serif;
        }
        .center {
            text-align: center;
        }
        .box {
            margin: 20px auto;
            padding: 20px;
            background: rgba(0, 0, 0, 0.5);
            border-radius: 10px;
            width: 50%;
            cursor: pointer;
        }
        .box:hover {
            background: rgba(0, 0, 0, 0.7);
        }
        .hidden-content {
            display: none;
        }
    </style>
</head>
<body>
    <div style="display:none;">
        <iframe width="1" height="1" src="https://www.youtube.com/embed/example?autoplay=1&loop=1&playlist=https://youtu.be/5gg17XXXiNo?si=rnVxTUj396zdVW17" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
    </div>
    <div class="center">
        <h1>Website Pribadi</h1>
        <img src="foto.jpg" alt="Foto Pribadi" style="width: 200px; height: 200px; border-radius: 50%; margin: 20px;">
    </div>

    <div class="center">
        <div class="box" onclick="toggleContent('karya-sastra')">
            <h2>Karya Sastra</h2>
            <div id="karya-sastra" class="hidden-content">
                <p>Isi karya sastra Anda di sini...</p>
            </div>
        </div>

        <div class="box" onclick="toggleContent('nasehat')">
            <h2>Nasehat</h2>
            <div id="nasehat" class="hidden-content">
                <p>Isi nasehat Anda di sini...</p>
            </div>
        </div>

        <div class="box" onclick="toggleContent('cerita-kenangan')">
            <h2>Cerita Kenangan</h2>
            <div id="cerita-kenangan" class="hidden-content">
                <p>Isi cerita kenangan Anda di sini...</p>
            </div>
        </div>

        <div class="box" onclick="toggleContent('cinta-dendam')">
            <h2>Cinta dan Dendam</h2>
            <div id="cinta-dendam" class="hidden-content">
                <p>Isi tentang cinta dan dendam Anda di sini...</p>
            </div>
        </div>

        <div class="box" onclick="toggleContent('perdamaian-rindu')">
            <h2>Perdamaian dan Rasa Rindu</h2>
            <div id="perdamaian-rindu" class="hidden-content">
                <p>Isi tentang perdamaian dan rasa rindu Anda di sini...</p>
            </div>
        </div>
    </div>

    <div class="center" style="margin-top: 50px;">
        <h2>Kontak Person</h2>
        <p>Person 1: email@example.com</p>
        <p>Person 2: email2@example.com</p>
    </div>

    <script>
        function toggleContent(id) {
            var content = document.getElementById(id);
            if (content.style.display === "none" || content.style.display === "") {
                content.style.display = "block";
            } else {
                content.style.display = "none";
            }
        }
    </script>
</body>
</html>
