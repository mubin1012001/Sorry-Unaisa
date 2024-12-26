<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>I’m Sorry</title>
    <style>
        body {
            font-family: 'Helvetica Neue', Arial, sans-serif;
            background: linear-gradient(135deg, #ffecec, #ffdee2);
            color: #333;
            text-align: center;
            margin: 0;
            padding: 0;
            animation: backgroundFade 8s infinite alternate;
        }

        @keyframes backgroundFade {
            0% { background: linear-gradient(135deg, #ffecec, #ffdee2); }
            100% { background: linear-gradient(135deg, #ffdee2, #ffecec); }
        }

        .card {
            max-width: 500px;
            margin: 50px auto;
            background: #fff;
            padding: 20px;
            border-radius: 15px;
            box-shadow: 0 4px 20px rgba(0, 0, 0, 0.3);
            border: 3px solid #f5c6cb;
            transition: transform 0.3s;
        }

        .card:hover {
            transform: scale(1.05);
        }

        img {
            max-width: 100%;
            border-radius: 10px;
            margin-bottom: 15px;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2);
            transition: box-shadow 0.3s;
        }

        img:hover {
            box-shadow: 0 6px 25px rgba(0, 0, 0, 0.4);
        }

        h1 {
            font-size: 32px;
            color: #d9534f;
            text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.3);
            animation: textGlow 1.5s infinite alternate;
        }

        @keyframes textGlow {
            0% { text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.3); }
            100% { text-shadow: 4px 4px 10px #d9534f; }
        }

        p {
            font-size: 16px;
            line-height: 1.8;
        }

        button {
            background-color: #007bff;
            color: white;
            border: none;
            padding: 12px 18px;
            font-size: 16px;
            border-radius: 8px;
            cursor: pointer;
            transition: background-color 0.3s, transform 0.3s;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
        }

        button:hover {
            background-color: #0056b3;
            transform: scale(1.1);
        }

        .surprise {
            background-color: #fff4e6;
            padding: 15px;
            border: 2px dashed #f5c6cb;
            border-radius: 10px;
            margin-top: 20px;
            animation: surpriseFade 3s infinite alternate;
        }

        @keyframes surpriseFade {
            0% { transform: scale(1); }
            100% { transform: scale(1.02); }
        }

        .surprise p {
            font-size: 18px;
            font-weight: bold;
            color: #d9534f;
        }

        .sparkle {
            font-size: 24px;
            color: #ffc107;
            animation: sparkle 1.5s infinite;
        }

        @keyframes sparkle {
            0% { opacity: 0.5; }
            50% { opacity: 1; }
            100% { opacity: 0.5; }
        }

        /* Music Icon */
        .music {
            margin-top: 20px;
        }

        .music button {
            background-color: #28a745;
            color: white;
            padding: 10px 15px;
            font-size: 14px;
            border-radius: 5px;
        }

        .music button:hover {
            background-color: #218838;
        }
    </style>
</head>
<body>
    <div class="card">
        <img src="/mnt/data/received_748534800267628.jpeg" alt="Apology">
        <h1>Forgive Me, Love</h1>
        <p>
            Look My love I know I made you sad... but you also know..when we argue or we fight how I feel...I just wanted you to text me... Trust me I would have waited until death... Moving to another girl is not my thing...loving you is the only thing I know...yes I doubted but trust me My love...It's just my fear of losing you...Other than you and my Family I don't fear losing anything not even my life...But I wanted to create something special. That's why I told Ohin to bring a cake...But at the last moment our plan flopped ☺☺... In My Story...You're my Only Wife...There will never be another woman in that position 😅....
        </p>
        <button onclick="alert('I promise to never take you for granted again. 💖')">Will You Forgive Me?</button>
        <div class="surprise">
            <p>Here’s a little surprise just for you!</p>
            <p class="sparkle">✨ You’re the most amazing person I know ✨</p>
            <p>
                Check your favorite playlist—I added a special song that reminds me of you.
                <br>Can’t wait to see that smile again! 😍
            </p>
        </div>
        <div class="music">
            <button onclick="playMusic()">Play Background Music</button>
            <audio id="bg-music" loop>
                <source src="/path-to-your-music-file.mp3" type="audio/mpeg">
                Your browser does not support the audio element.
            </audio>
        </div>
    </div>

    <script>
        function playMusic() {
            const music = document.getElementById('bg-music');
            if (music.paused) {
                music.play();
            } else {
                music.pause();
            }
        }
    </script>
</body>
</html>
