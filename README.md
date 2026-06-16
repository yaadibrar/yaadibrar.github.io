<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>A Special Surprise for Jashan ❤️</title>
    <link href="https://fonts.googleapis.com/css2?family=Fredoka+One&family=Quicksand:wght@500;700&display=swap" rel="stylesheet">
    
    <style>
        /* Base Styling & Background Wall Theme */
        body {
            font-family: 'Quicksand', sans-serif;
            background-color: #fff0f5; /* Soft Lavender Blush */
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

        /* Background Wall Deco (Balloons & Hearts) */
        .wall-deco {
            position: absolute;
            font-size: 50px;
            opacity: 0.25;
            user-select: none;
            pointer-events: none;
            z-index: 1;
        }

        /* Glassmorphism Card (Lovely Soft Look) */
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

        .hidden {
            display: none !important;
        }

        h2 { 
            font-family: 'Fredoka One', cursive;
            color: #d81b60; 
            margin-bottom: 20px;
            text-shadow: 1px 1px 2px rgba(0,0,0,0.05);
            font-size: 26px;
            letter-spacing: 0.5px;
        }
        
        p { 
            color: #6d4c41; 
            line-height: 1.6; 
            font-size: 19px; 
            font-weight: 700;
        }

        /* Inputs */
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
            transition: border-color 0.3s;
        }
        input[type="password"]:focus {
            border-color: #e91e63;
        }

        /* Lovely Rounded Buttons */
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
            transition: transform 0.2s, box-shadow 0.2s, background 0.2s;
            margin: 10px;
        }
        button:hover { 
            background: linear-gradient(135deg, #e91e63, #c2185b);
            transform: translateY(-3px) scale(1.03); 
            box-shadow: 0 8px 20px rgba(233, 30, 99, 0.4);
        }

        /* Captcha Box Style */
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

        /* Images & Stickers */
        .gif-display { width: 160px; height: 160px; margin-bottom: 20px; object-fit: contain; }
        
        .bday-image { 
            width: 210px; 
            height: 210px; 
            border-radius: 25px; 
            border: 6px solid #fff; 
            box-shadow: 0 8px 20px rgba(216, 27, 96, 0.25); 
            margin-bottom: 20px; 
            object-fit: cover; 
        }
        
        .dog-stickers-container { display: flex; justify-content: space-around; margin: 25px 0; gap: 10px; }
        .dog-stickers-container img { 
            width: 30%; 
            height: 110px; 
            border-radius: 15px; 
            object-fit: contain; 
            background: #fffafc; 
            border: 2px dashed #ffb6c1; 
            padding: 5px; 
            box-shadow: 0 4px 10px rgba(0,0,0,0.03);
        }

        /* Envelope */
        .envelope { font-size: 85px; cursor: pointer; transition: transform 0.3s; display: inline-block; }
        .envelope:hover { transform: scale(1.15) rotate(-5deg); }

        /* Floating Stickers (Live Generation) */
        .sticker {
            position: absolute;
            bottom: -50px;
            font-size: 32px;
            cursor: default;
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
        <img class="gif-display" src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExbWdtcm93YThndm95Z3VwY2N5bWZndWZ0amZ6N293bXp5NjZpYmdpayZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9cw/9fUVkwgxoFfAvFgG33/giphy.gif" alt="Puppy holding flower">
        <h2>HEY JASHAN!! <br>I made something for you.<br>Do you want to see?</h2>
        <button onclick="nextStep(3)">Yes</button>
        <button id="noBtn" onclick="tryClickNo()">No</button>
    </div>

    <div id="stepAngry" class="card hidden">
        <img class="gif-display" src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExM3Z0MzdpaXN4YnY2dnB0ZmluYnVvNzU3ZzNiaWZ3Y3FubXozN3VvdyZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9cw/WwG96v7fPn8T2Vp7Ie/giphy.gif" alt="Angry puppy">
        <h2>HOW DARE YOU! 😂</h2>
        <button onclick="backToQuestion()">Go back and pick Yes! 💖</button>
    </div>

    <div id="step3" class="card hidden">
        <img class="bday-image" src="https://i.ibb.co/nq00DJVK/1781543226140.png" alt="Birthday Special Photo">
        <h2>HAPPY BIRTHDAY JASHAN! 💖</h2>
        <p>You are my favorite notification.<br>Stay cute, stay happy, stay mine. 🎀</p>
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
            "Lao Madam ji Khaas wish tuhade lyi"
        </p>
        
        <div class="dog-stickers-container">
            <img src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExNmtpbnkyajA5Y2I4eHh3NmIxcTZvMzJpcWtzMW13MXV1MmhuZTA2MCZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9cw/WwA7266V2p9D8rR9Oq/giphy.gif" alt="Birthday Dog 1">
            <img src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExYzRiaWR3dzN6MmVwOGxtZHdyZ3l1b2x0cmhjd3d4aWgyc3ExNHoxdSZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9cw/gImsKzPrc8v4fS76b0/giphy.gif" alt="Birthday Dog 2">
            <img src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExMXU5ZWwyc3RtdzUzdzZ5a3Jid3d4ZHpnemw4bWszcmhvb3owNWt4byZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9cw/jUon4P3xHhAEvpOfK3/giphy.gif" alt="Birthday Dog 3">
        </div>
        <button onclick="nextStep(6)">Click here</button>
    </div>

    <div id="step6" class="card hidden">
        <h2>Here's a final surprise for you!!!</h2>
        <img class="gif-display" src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExMzY5Y2w2Z3RnaTZvdnpteXUybTFhZXAybGZ5Z240MHhtdmRjMmRhNCZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9cw/L32gqR8zG38LqV8L4K/giphy.gif" alt="Gift box" style="cursor: pointer; width: 180px; height: 180px;" onclick="triggerFinalSurprise()">
        <p>Tap the gift box to open it!</p>
    </div>

    <div id="step7" class="card hidden">
        <h2>Here is a surprise for you!!! 🎁🌟</h2>
        <img class="gif-display" src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExbWwxdGg1ZzdicTJwNXg1M3gzMGxnd2dzYTM3dW5pdmluZTh0amxjOCZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9cw/9unqM66sC536G4DcoG/giphy.gif" alt="Cute mocha bear hug" style="width: 230px; height: 230px; margin-bottom: 10px;">
        <h2>Here is virtual hug for you 🤗</h2>
        <p style="font-weight: bold; color: #d81b60; font-size: 20px;">I love you to the moon and back!</p>
    </div>

    <script>
        // --- ⚙️ CUSTOMIZATION CONFIGURATION ⚙️ ---
        const CORRECT_PASSWORD = "yaadi's surprise"; 
        
        // 🎵 ਇੱਥੇ ਆਪਣਾ YouTube Video ID ਪਾਓ 
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

        function backToQuestion() {
            nextStep(2);
        }

        // Live Floating Stickers Generator (Balloons & Hearts Burst)
        function startStickers() {
            const stickerTypes = ['🎈', '💖', '🎂', '🎈', '🧸', '✨', '🌸', '❤️', '🥰', '🎈'];
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
