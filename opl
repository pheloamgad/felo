<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>حقك عليا يا طمطم ❤️</title>
    <link href="https://fonts.googleapis.com/css2?family=Cairo:wght@400;700&display=swap" rel="stylesheet">
    <style>
        body {
            background-color: #fff5f7;
            font-family: 'Cairo', sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            overflow: hidden;
            text-align: center;
        }
        .container {
            background: white;
            padding: 30px;
            border-radius: 25px;
            box-shadow: 0 10px 25px rgba(0,0,0,0.1);
            max-width: 400px;
            width: 90%;
            position: relative;
            z-index: 10;
        }
        h1 { color: #ad1457; font-size: 1.8rem; margin-bottom: 10px; }
        p { color: #666; line-height: 1.6; font-size: 1.1rem; }
        .btns { margin-top: 30px; display: flex; flex-direction: column; gap: 15px; align-items: center; position: relative; height: 120px; }
        
        .btn {
            padding: 12px 25px;
            border: none;
            border-radius: 50px;
            font-weight: bold;
            cursor: pointer;
            transition: 0.3s;
            font-family: 'Cairo';
        }
        .btn-yes { background: #d81b60; color: white; width: 220px; z-index: 100; box-shadow: 0 4px 15px rgba(216, 27, 96, 0.3); }
        .btn-no { background: #eee; color: #888; position: absolute; transition: 0.1s; }

        .sad-emoji { font-size: 50px; margin-bottom: 10px; animation: bounce 2s infinite; }
        @keyframes bounce { 0%, 100% { transform: translateY(0); } 50% { transform: translateY(-10px); } }
    </style>
</head>
<body>

    <iframe id="music-player" width="0" height="0" src="https://www.youtube.com/embed/x3mNbsQk3PI?autoplay=1&enablejsapi=1" frameborder="0" style="display:none;"></iframe>

    <div class="container">
        <div class="sad-emoji">🥺</div>
        <h1>صالحيني يا طمطم..</h1>
        <p>
            أغلى إنسانة في حياتي زعلانة مني؟ <br>
            والله الدنيا وحشة من غير ضحكتك. <br>
            <b>تسامحيني ونرجع أحسن من الأول؟</b>
        </p>

        <div class="btns">
            <button class="btn btn-yes" onclick="celebrate()">خلاص سامحتك يا حبيب قلبي ❤️</button>
            <button class="btn btn-no" id="no-btn" onmouseover="moveButton()">لأ لسه زعلانة 😤</button>
        </div>
    </div>

    <script src="https://cdn.jsdelivr.net/npm/canvas-confetti@1.5.1/dist/confetti.browser.min.js"></script>
    <script>
        // دالة تحريك زرار الرفض
        function moveButton() {
            const btn = document.getElementById('no-btn');
            const x = Math.random() * (window.innerWidth - btn.offsetWidth);
            const y = Math.random() * (window.innerHeight - btn.offsetHeight);
            btn.style.position = 'fixed';
            btn.style.left = x + 'px';
            btn.style.top = y + 'px';
        }

        // احتفال الصلح
        function celebrate() {
            const container = document.querySelector('.container');
            container.innerHTML = `
                <div style="font-size: 60px;">💖</div>
                <h1 style="color: #d81b60;">عاشت طمطم اللي قلبها أبيض!</h1>
                <p>وعد عليا ما أزعلِك تاني يا ملكة قلبي.. <br> بحبك أوي ❤️</p>
                <div style="font-size: 40px;">👑👑</div>
            `;
            
            // ورق ملون
            var duration = 10 * 1000;
            var animationEnd = Date.now() + duration;
            var defaults = { startVelocity: 30, spread: 360, ticks: 60, zIndex: 0 };

            var interval = setInterval(function() {
                var timeLeft = animationEnd - Date.now();
                if (timeLeft <= 0) return clearInterval(interval);
                confetti(Object.assign({}, defaults, { particleCount: 50, origin: { x: Math.random(), y: Math.random() - 0.2 } }));
            }, 250);
        }

        // تشغيل الموسيقى تلقائياً (تنبيه: بعض المتصفحات تطلب ضغطة من المستخدم أولاً)
        window.addEventListener('click', function() {
            const player = document.getElementById('music-player');
            player.src += "&autoplay=1";
        }, { once: true });
    </script>
</body>
</html>
