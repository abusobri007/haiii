<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interactive 3D Book</title>
    <style>
        body {
            margin: 0;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background: linear-gradient(to right, #c9d6ff, #e2e2e2);
            overflow: hidden;
        }
        .book {
            width: 320px;
            height: 420px;
            perspective: 1500px;
            position: relative;
        }
        .cover, .page {
            position: absolute;
            width: 100%;
            height: 100%;
            border-radius: 5px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
        }
        .cover {
            background: linear-gradient(to right, #f8b195, #f67280);
            color: #fff;
            font-size: 32px;
            font-weight: bold;
            display: flex;
            justify-content: center;
            align-items: center;
            cursor: pointer;
            transform-origin: left;
            transform: rotateY(0deg);
            transition: transform 1.2s cubic-bezier(0.68, -0.55, 0.27, 1.55);
            z-index: 4;
        }
        .page {
            transform-origin: left;
            transform: rotateY(0deg);
            background: #fff;
            transition: transform 1s ease-in-out;
        }
        .page img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            border-radius: 5px;
        }
        .page:last-child {
            display: flex;
            justify-content: center;
            align-items: center;
            font-size: 32px;
            font-weight: bold;
            color: #f67280;
            text-align: center;
            padding: 20px;
        }
        .page:nth-child(2) {
            z-index: 3;
        }
        .page:nth-child(3) {
            z-index: 2;
        }
        .page:nth-child(4) {
            z-index: 1;
        }
        .page.open {
            transform: rotateY(-180deg);
        }
    </style>
</head>
<body>
    <div class="book">
        <div class="cover" onclick="openCover()">Open Book</div>
        <div class="page" onclick="togglePage(this)">
            <img src="nina.jpg" alt="Person 1">
        </div>
        <div class="page" onclick="togglePage(this)">
            <img src="nina2.jpg" alt="Person 2">
        </div>
        <div class="page" onclick="togglePage(this)">
            <img src="nina3.jpg" alt="Person 3">
        </div>
        <div class="page" onclick="togglePage(this)">
            Good Morning Cantikkkkkk 🌸✨
        </div>
    </div>

    <audio id="backgroundMusic" loop>
        <source src="lagu.mp3" type="audio/mpeg">
        Your browser does not support the audio element.
    </audio>

    <script>
        function openCover() {
            const cover = document.querySelector('.cover');
            cover.style.transform = 'rotateY(-180deg)';
        }

        function togglePage(page) {
            page.classList.toggle('open');
        }

        // Play background music on first click
        document.body.addEventListener('click', () => {
            const music = document.getElementById('backgroundMusic');
            if (music.paused) {
                music.play();
            }
        });
    </script>
</body>
</html>
