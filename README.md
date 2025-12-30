<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>For My Bacha 🌸</title>
    <link href="https://fonts.googleapis.com/css2?family=Dancing+Script:wght@600&family=Quicksand:wght@400;500&display=swap" rel="stylesheet">
    <style>
        :root {
            --pale-pink: #fff0f3;
            --marshmallow: #ffffff;
            --soft-gold: #efd389;
            --text-grey: #5a5a5a;
            --accent: #ff8fa3;
        }

        body, html {
            margin: 0; padding: 0;
            background: radial-gradient(circle, #ffffff 0%, #fff0f3 100%);
            color: var(--text-grey);
            font-family: 'Quicksand', sans-serif;
            text-align: center;
            overflow: hidden;
        }

        .bg-elements { position: fixed; top: 0; left: 0; width: 100%; height: 100%; pointer-events: none; z-index: 0; }
        .floating { position: absolute; color: rgba(255, 143, 163, 0.2); animation: floatUp 6s linear infinite; }
        @keyframes floatUp {
            0% { transform: translateY(110vh) rotate(0deg); opacity: 1; }
            100% { transform: translateY(-10vh) rotate(360deg); opacity: 0; }
        }

        .screen {
            display: none; position: relative; z-index: 1;
            min-height: 100vh; flex-direction: column;
            align-items: center; justify-content: center;
            padding: 20px; animation: fadeIn 0.8s ease;
        }
        .active { display: flex; }
        @keyframes fadeIn { from { opacity: 0; transform: scale(0.98); } to { opacity: 1; transform: scale(1); } }

        h1 { font-family: 'Dancing Script', cursive; font-size: 2.2rem; color: var(--accent); margin-bottom: 15px; }
        
        .memory-card {
            background: rgba(255, 255, 255, 0.85);
            padding: 25px; border-radius: 35px;
            max-width: 90%; max-height: 65vh; overflow-y: auto;
            box-shadow: 0 10px 30px rgba(255, 182, 193, 0.15);
            text-align: left; border: 2px solid #fff;
        }

        .memory-item { margin-bottom: 20px; border-bottom: 1px solid #fff0f3; padding-bottom: 10px; }
        .memory-item:last-child { border: none; }
        .memory-item h3 { font-size: 1rem; color: var(--accent); margin: 0 0 5px 0; }
        .memory-item p { font-size: 0.85rem; margin: 0; line-height: 1.5; color: #666; }

        .btn {
            margin-top: 20px; padding: 12px 35px;
            background: var(--accent); color: white;
            border: none; border-radius: 50px;
            font-weight: 500; cursor: pointer;
            box-shadow: 0 5px 15px rgba(255, 143, 163, 0.3);
        }

        .ticket {
            background: white; padding: 30px; border-radius: 20px;
            border: 2px dashed var(--soft-gold);
            box-shadow: 0 8px 20px rgba(239, 211, 137, 0.2);
        }
    </style>
</head>
<body>

    <div class="bg-elements" id="bg"></div>

    <div id="p1" class="screen active">
        <h1>Happy New Year, Bacha ✨</h1>
        <p>A surprise for my beautiful Ishita</p>
        <button class="btn" onclick="show(2)">Open My Letter 🕊️</button>
    </div>

    <div id="p2" class="screen">
        <h1>My Dearest Bbu... 🌸</h1>
        <div class="memory-card" style="text-align: center;">
            <p>As I look back at everything that happened this year, there is one thing that stands out above all the rest. You.</p>
            <p>In 2025, I found the bestest person I have ever known. Since the moment we met, my world has become so much better in every single way. You brought a joy into my life that I never knew was possible.</p>
            <p>Thank you for being my girl, my light, and my everything. I am so thankful to have you by my side.</p>
        </div>
        <button class="btn" onclick="show(3)">Our Recap 🪄</button>
    </div>

    <div id="p3" class="screen">
        <h1>Cherished Times 🪄</h1>
        <div class="memory-card">
            <div class="memory-item">
                <h3>🏏 The RCB Final Match</h3>
                <p>The day of closeness to us.</p>
            </div>
            <div class="memory-item">
                <h3>🙏 Ganesh Chaturthi</h3>
                <p>From the prayers to the Visarjan, sharing these spiritual moments with you was magical.</p>
            </div>
            <div class="memory-item">
                <h3>💃 Our Navratri Nights</h3>
                <p>The 4 AM roads and dancing until the sky turned light—happiness that never faded.</p>
            </div>
            <div class="memory-item">
                <h3>🎂 Joyful Birthdays</h3>
                <p>Celebrating Mumma, Daddy, and Rudu’s birthdays with so much love and laughter.</p>
            </div>
            <div class="memory-item">
                <h3>🏰 Udaipur Trip</h3>
                <p>Our long drives through Rajasthan—moments of us that I'll cherish forever.</p>
            </div>
        </div>
        <button class="btn" onclick="show(4)">More Memories 🍬</button>
    </div>

    <div id="p4" class="screen">
        <h1>Little Moments, Big Love 🍬</h1>
        <div class="memory-card">
            <div class="memory-item">
                <h3>🚇 The Metro Station</h3>
                <p>Where I used to wait just to see you—now we ride the same metro together every day.</p>
            </div>
            <div class="memory-item">
                <h3>🎮 Arcade, Bowling & Karting</h3>
                <p>The thrill of being competitive and racing on the track together—every game was a win with you.</p>
            </div>
            <div class="memory-item">
                <h3>🍦 Bunking for Ice Cream</h3>
                <p>Skipping Garba class just to have ice cream and fun—no regrets, only memories.</p>
            </div>
            <div class="memory-item">
                <h3>🏎️ Our Long Drives</h3>
                <p>Just us, the open road, and endless conversations. Every mile with you is my favorite.</p>
            </div>
            <div class="memory-item">
                <h3>🤝 Hand Holding</h3>
                <p>Those random, cute moments holding hands in the car—it's just too cute.</p>
            </div>
        </div>
        <button class="btn" onclick="show(5)">Wait, one more thing... 🎁</button>
    </div>

    <div id="p5" class="screen">
        <div class="ticket">
            <p style="font-size: 0.7rem; letter-spacing: 2px; color: #ccb;">GOLDEN TICKET</p>
            <h2 style="font-family: 'Dancing Script'; color: var(--soft-gold); font-size: 2rem; margin: 10px 0;">100 Hugs & 100 Kisses 💋</h2>
            <p>For: <b>Ishita</b></p>
            <p style="font-size: 10px; color: #ddd; margin-top: 10px;">Unlimited Use • Valid Forever</p>
        </div>
        <button class="btn" onclick="show(6)">Final Message 🥂</button>
    </div>

    <div id="p6" class="screen">
        <h1>Welcome to 2026, Bacha 🥂</h1>
        <div class="memory-card" style="text-align: center;">
            <p>Just like we enjoyed 2025 together, let's make 2026 exactly the same—with more laughter and love.</p>
            <p>I'm so excited to spend another 365 days with my best person.</p>
            <h2 style="font-family: 'Dancing Script'; color: var(--accent);">I Love You Forever ❤️</h2>
        </div>
        <button class="btn" onclick="location.reload()">See Again ✨</button>
    </div>

    <script>
        function show(num) {
            document.querySelectorAll('.screen').forEach(s => s.classList.remove('active'));
            document.getElementById('p' + num).classList.add('active');
        }

        function createHeart() {
            const h = document.createElement('div');
            h.classList.add('floating');
            h.innerHTML = '❤️';
            h.style.left = Math.random() * 100 + 'vw';
            h.style.fontSize = Math.random() * 20 + 10 + 'px';
            h.style.animationDuration = Math.random() * 3 + 3 + 's';
            document.getElementById('bg').appendChild(h);
            setTimeout(() => h.remove(), 6000);
        }
        setInterval(createHeart, 400);
    </script>
</body>
</html>
