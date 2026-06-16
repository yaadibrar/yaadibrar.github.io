<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>A Special Surprise for Jashan ❤️</title>
    <link href="https://fonts.googleapis.com/css2?family=Fredoka+One&family=Quicksand:wght@500;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Quicksand', sans-serif;
            background-color: #fff0f5;
            background-image: 
                radial-gradient(#ffb6c1 10%, transparent 11%),
                radial-gradient(#ffb6c1 10%, transparent 11%);
            background-size: 60px 60px;
            background-position: 0 0, 30px 30px;
            margin: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            overflow: hidden;
            position: relative;
        }

        .wall-deco {
            position: absolute;
            font-size: 50px;
            opacity: 0.25;
            user-select: none;
            pointer-events: none;
            z-index: 1;
        }

        .card {
            background: rgba(255, 255, 255, 0.85);
            backdrop-filter: blur(10px);
            -webkit-backdrop-filter: blur(10px);
            border: 2px solid rgba(255, 182, 193, 0.6);
            border-radius: 30px;
            box-shadow: 0 15px 35px rgba(216, 27, 96, 0.15);
            padding: 40px;
            text-align: center;
            max-width: 420px;
            width: 85%;
            transition: all 0.5s cubic-bezier(0.175, 0.885, 0.32, 1.275);
            z-index: 10;
        }

        .hidden { display: none !important; }

        h2 { 
            font-family: 'Fredoka One', cursive;
            color: #d81b60; 
            margin-bottom: 20px;
            text-shadow: 1px 1px 2px rgba(0,0,0,0.05);
            font-size: 26px;
        }
        
        p { color: #6d4c41; line-height: 1.6; font-size: 19px; font-weight: 700; }

        input[type="password"] {
            font-family: 'Quicksand', sans-serif;
            padding: 12px; 
            width: 80%; 
            border-radius: 15px; 
            border: 2px solid #ffb6c1; 
            margin-bottom: 20px; 
            text-align: center;
            font-size: 16px;
            font-weight: bold;
            color: #d81b60;
            outline: none;
            background-color: #fffafb;
        }

        button {
            font-family: 'Quicksand', sans-serif;
            background: linear-gradient(135deg, #ff4081, #ec407a);
            color: white;
            border: none;
            padding: 14px 32px;
            font-size: 17px;
            border-radius: 50px;
            cursor: pointer;
            font-weight: bold;
            box-shadow: 0 5px 15px rgba(233, 30, 99, 0.3);
            transition: transform 0.2s, box-shadow 0.2s;
            margin: 10px;
        }
        button:hover { 
            background: linear-gradient(135deg, #e91e63, #c2185b);
            transform: translateY(-3px) scale(1.03); 
        }

        .captcha-container {
            border: 2px dashed #ffb6c1;
            background: #fffafb;
            padding: 10px 20px;
            display: inline-flex;
            align-items: center;
            border-radius: 15px;
            margin-bottom: 20px;
        }
        .captcha-checkbox { margin-right: 15px; width: 22px; height: 22px; cursor: pointer; accent-color: #e91e63; }

        /* 🎪 Code Generated Animated Stickers (Will Never Block!) */
        .animated-emoji {
            font-size: 100px;
            margin-bottom: 20px;
            display: inline-block;
            animation: bounce-wiggle 2s infinite ease-in-out;
        }

        @keyframes bounce-wiggle {
            0%, 100% { transform: translateY(0) rotate(0deg); }
            50% { transform: translateY(-15px) rotate(8deg); }
        }

        .bday-image { 
            width: 210px; 
            height: 210px; 
            border-radius: 25px; 
            border: 6px solid #fff; 
            box-shadow: 0 8px 20px rgba(216, 27, 96, 0.25); 
            margin-bottom: 20px; 
            object-fit: cover; 
        }
        
        /* 🐾 3 Dog Custom Stickers Display */
        .dog-stickers-container { display: flex; justify-content: space-around; margin: 25px 0; gap: 10px; }
        .dog-sticker {
            font-size: 55px;
            background: #fffafc; 
            border: 2px dashed #ffb6c1; 
            padding: 10px;
            border-radius: 20px;
            width: 25%;
            animation: dance 1.5s infinite ease-in-out alternate;
        }
        .dog-sticker:nth-child(2) { animation-delay: 0.3s; }
        .dog-sticker:nth-child(3) { animation-delay: 0.6s; }

        @keyframes dance {
            0% { transform: scale(0.9) rotate(-5deg); }
            100% { transform: scale(1.1) rotate(5deg); }
        }

        .envelope { font-size: 85px; cursor: pointer; transition: transform 0.3s; display: inline-block; animation: pulse 2s infinite; }
        @keyframes pulse {
            0%, 100% { transform: scale(1); }
            50% { transform: scale(1.08); }
        }
        .envelope:hover { transform: scale(1.15) rotate(-5deg); }

        .sticker {
            position: absolute;
            bottom: -50px;
            font-size: 32px;
            user-select: none;
            pointer-events: none;
            animation: floatUp 4.2s linear forwards;
            z-index: 2;
        }

        @keyframes floatUp {
            0% { transform: translateY(0) translateX(0) rotate(0deg); opacity: 1; }
            100% { transform: translateY(-105vh) translateX(60px) rotate(360deg); opacity: 0; }
        }
        #musicPlayer { position: absolute; width: 1px; height: 1px; opacity: 0; pointer-events: none; }
    </style>
</head>
<body>

    <div class="wall-deco" style="top: 10%; left: 8%;">🎈</div>
    <div class="wall-deco" style="top: 15%; left: 12%;">🎈</div>
    <div class="wall-deco" style="top: 8%; right: 10%;">🎈</div>
    <div class="wall-deco" style="top: 20%; right: 5%;">🎈</div>
    <div class="wall-deco" style="bottom: 15%; left: 5%;">💖</div>
    <div class="wall-deco" style="bottom: 10%; right: 8%;">💖</div>

    <div id="musicPlayer"></div>

    <div id="step1" class="card">
        <h2>Enter the password to view</h2>
        <input type="password" id="passwordInput" placeholder="Enter password..."><br>
        <div class="captcha-container">
            <input type="checkbox" id="captchaBox" class="captcha-checkbox">
            <span style="font-size: 15px; color: #6d4c41; font-weight: bold;">I'm not a robot</span>
        </div><br>
        <button onclick="checkStep1()">Continue</button>
    </div>

    <div id="step2" class="card hidden">
        <div class="animated-emoji">🐶💐</div>
        <h2>HEY JASHAN!! <br>I made something for you.<br>Do you want to see?</h2>
        <button onclick="nextStep(3)">Yes</button>
        <button id="noBtn" onclick="tryClickNo()">No</button>
    </div>

    <div id="stepAngry" class="card hidden">
        <div class="animated-emoji">😤🐕</div>
        <h2>HOW DARE YOU! 😂</h2>
        <button onclick="backToQuestion()">Go back and pick Yes! 💖</button>
    </div>

    <div id="step3" class="card hidden">
        <img class="bday-image" src="https://i.ibb.co/nq00DJVK/1781543226140.png">
        <h2>HAPPY BIRTHDAY JASHAN! 💖</h2>
        <p>You are not a headache,you are my favorite notification.<br>Stay cute, stay happy, stay mine. 🎀</p>
        <button onclick="nextStep(4)">Next</button>
    </div>

    <div id="step4" class="card hidden">
        <h2>You have a letter ✉️</h2>
        <div class="envelope" onclick="nextStep(5)">💌</div>
        <p style="font-size: 15px; color: #888; margin-top: 20px; font-weight: bold;">Tap the letter to open</p>
    </div>

    <div id="step5" class="card hidden">
        <h2>My Letter to You 💕</h2>
        <p style="font-size: 23px; font-weight: bold; color: #d81b60; margin-bottom: 25px; font-family: 'Fredoka One', cursive;">
            "Lao Madam ji Khaas wish tuhade lyi,kuch bnaaya tere lyi YouTube te check kar la"
        </p>
        <div class="dog-stickers-container">
            <div class="dog-sticker">🐶🎂</div>
            <div class="dog-sticker">🐕🎈</div>
            <div class="dog-sticker">🦮🎉</div>
        </div>
        <button onclick="nextStep(6)">Click here</button>
    </div>

    <div id="step6" class="card hidden">
        <h2>Here's a final surprise for you!!!</h2>
        <div class="animated-emoji" style="cursor: pointer; font-size: 110px;" onclick="triggerFinalSurprise()">🎁</div>
        <p>Tap the gift box to open it!</p>
    </div>

    <div id="step7" class="card hidden">
        <h2>Here is a surprise for you!!! 🎁🌟</h2>
        <div class="animated-emoji" style="font-size: 120px;">🧸🤗</div>
        <h2>Here is virtual hug for you 🤗</h2>
        <p style="font-weight: bold; color: #d81b60; font-size: 20px;">I love you to the moon and back!</p>
    </div>

    <script>
        const CORRECT_PASSWORD = "yaadi's surprise"; 
        
        // 🎵 ਇੱਥੇ ਆਪਣਾ YouTube Video ID ਪਾਓ (ਜਿਵੇਂ "dQw4w9WgXcQ")
        const YOUTUBE_VIDEO_ID = "dQw4w9WgXcQ"; 

        let stickerInterval;

        function checkStep1() {
            const passwordEntered = document.getElementById('passwordInput').value.toLowerCase().trim();
            const captchaChecked = document.getElementById('captchaBox').checked;

            if (passwordEntered === CORRECT_PASSWORD && captchaChecked) {
                nextStep(2);
                startStickers(); 
            } else if (passwordEntered !== CORRECT_PASSWORD) {
                alert("Wrong password! Hint: Check the capitalization/spacing.");
            } else {
                alert("Please check the 'I'm not a robot' box!");
            }
        }

        function triggerFinalSurprise() {
            nextStep(7);
            const playerDiv = document.getElementById('musicPlayer');
            playerDiv.innerHTML = `<iframe src="https://www.youtube.com/embed/${YOUTUBE_VIDEO_ID}?autoplay=1&loop=1&playlist=${YOUTUBE_VIDEO_ID}" allow="autoplay"></iframe>`;
        }

        function nextStep(stepNumber) {
            document.querySelectorAll('.card').forEach(card => card.classList.add('hidden'));
            document.getElementById('step' + stepNumber).classList.remove('hidden');
        }

        function tryClickNo() {
            document.querySelectorAll('.card').forEach(card => card.classList.add('hidden'));
            document.getElementById('stepAngry').classList.remove('hidden');
        }

        function backToQuestion() { nextStep(2); }

        function startStickers() {
            const stickerTypes = ['🎈', '💖', '🎂', '🎈', '🧸', '✨', '🌸', '❤️', '🥰'];
            stickerInterval = setInterval(() => {
                const sticker = document.createElement('div');
                sticker.classList.add('sticker');
                sticker.innerText = stickerTypes[Math.floor(Math.random() * stickerTypes.length)];
                sticker.style.left = Math.random() * 100 + "vw";
                sticker.style.fontSize = Math.floor(Math.random() * 18 + 22) + "px";
                document.body.appendChild(sticker);
                setTimeout(() => { sticker.remove(); }, 4200);
            }, 350);
        }
    </script>
</body>
</html>
