<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>A Special Surprise for You ❤️</title>
    <style>
        /* Base Styling */
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background-color: #fce4ec;
            margin: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            overflow: hidden;
        }

        .card {
            background-color: white;
            border-radius: 20px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
            padding: 40px;
            text-align: center;
            max-width: 450px;
            width: 90%;
            transition: all 0.5s ease;
        }

        .hidden {
            display: none !important;
        }

        h2 { color: #d81b60; margin-bottom: 20px; }
        p { color: #555; line-height: 1.6; }

        /* Buttons */
        button {
            background-color: #e91e63;
            color: white;
            border: none;
            padding: 12px 28px;
            font-size: 16px;
            border-radius: 50px;
            cursor: pointer;
            font-weight: bold;
            transition: transform 0.2s, background-color 0.2s;
            margin: 10px;
        }
        button:hover { background-color: #c2185b; transform: scale(1.05); }

        /* Captcha Box Mockup */
        .captcha-container {
            border: 1px solid #ccc;
            background: #f9f9f9;
            padding: 10px 20px;
            display: inline-flex;
            align-items: center;
            border-radius: 3px;
            margin-bottom: 20px;
        }
        .captcha-checkbox { margin-right: 15px; width: 24px; height: 24px; cursor: pointer; }

        /* Image Sizing */
        .gif-display { width: 150px; height: 150px; margin-bottom: 20px; object-fit: contain; }
        .photo-gallery { display: flex; justify-content: space-around; margin: 20px 0; gap: 10px; }
        .photo-gallery img { width: 30%; border-radius: 8px; border: 4px solid white; box-shadow: 0 4px 8px rgba(0,0,0,0.2); }

        /* Envelope */
        .envelope { font-size: 80px; cursor: pointer; transition: transform 0.3s; }
        .envelope:hover { transform: scale(1.1) rotate(-5deg); }
    </style>
</head>
<body>

    <!-- STEP 1: Password & Captcha Screen -->
    <div id="step1" class="card">
        <h2>Enter the password to view</h2>
        <input type="password" id="passwordInput" placeholder="Hint: Her favorite nickname" style="padding: 10px; width: 80%; border-radius: 5px; border: 1px solid #ccc; margin-bottom: 20px; text-align: center;"><br>
        
        <div class="captcha-container">
            <input type="checkbox" id="captchaBox" class="captcha-checkbox">
            <span style="font-size: 14px; color: #555;">I'm not a robot</span>
        </div><br>
        
        <button onclick="checkStep1()">Continue</button>
    </div>

    <!-- STEP 2: The Question (Yes / No) -->
    <div id="step2" class="card hidden">
        <img class="gif-display" src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExbWdtcm93YThndm95Z3VwY2N5bWZndWZ0amZ6N293bXp5NjZpYmdpayZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9cw/9fUVkwgxoFfAvFgG33/giphy.gif" alt="Puppy holding flower">
        <h2>HEY!! I made something for you.<br>Do you want to see?</h2>
        <button onclick="nextStep(3)">Yes</button>
        <button id="noBtn" onclick="tryClickNo()">No</button>
    </div>

    <!-- STEP 2.5: Angry Dog if they clicked No -->
    <div id="stepAngry" class="card hidden">
        <img class="gif-display" src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExM3Z0MzdpaXN4YnY2dnB0ZmluYnVvNzU3ZzNiaWZ3Y3FubXozN3VvdyZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9cw/WwG96v7fPn8T2Vp7Ie/giphy.gif" alt="Angry puppy">
        <h2>HOW DARE YOU! 😂</h2>
        <button onclick="backToQuestion()">Go back and pick the right option</button>
    </div>

    <!-- STEP 3: Birthday Celebration Greeting -->
    <div id="step3" class="card hidden">
        <img class="gif-display" src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExYzh0MXM0aXptMXp5Z2thd3I2NWhreXNpeHpxejN4MGtkdmc1dmVheiZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9cw/H3X3UorInO2q0bMv14/giphy.gif" alt="Party Puppy">
        <h2>HAPPY BIRTHDAY BBG! 💖</h2>
        <p>You are my favorite notification.<br>Stay cute, stay happy, stay mine. 🎀</p>
        <button onclick="nextStep(4)">Next</button>
    </div>

    <!-- STEP 4: Letter Envelope -->
    <div id="step4" class="card hidden">
        <h2>You have a letter ✉️</h2>
        <div class="envelope" onclick="nextStep(5)">💌</div>
        <p style="font-size: 14px; color: #888; margin-top: 20px;">Tap the letter to open</p>
    </div>

    <!-- STEP 5: Letter Content & Mini Gallery -->
    <div id="step5" class="card hidden">
        <h2>My Letter to You 💕</h2>
        <p><em>"You are seen, you are heard, and you are loved, no matter what. If you ever feel unloved, remember that my love for you is boundless and endless."</em></p>
        
        <!-- Replace URLs with real photos of you two -->
        <div class="photo-gallery">
            <img src="https://via.placeholder.com/150" alt="Memory 1">
            <img src="https://via.placeholder.com/150" alt="Memory 2">
            <img src="https://via.placeholder.com/150" alt="Memory 3">
        </div>
        <button onclick="nextStep(6)">Click here</button>
    </div>

    <!-- STEP 6: Virtual Gift Box -->
    <div id="step6" class="card hidden">
        <h2>Here's a final surprise for you!!!</h2>
        <img class="gif-display" src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExM3Y5Y2w2Z3RnaTZvdnpteXUybTFhZXAybGZ5Z240MHhtdmRjMmRhNCZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9cw/L32gqR8zG38LqV8L4K/giphy.gif" alt="Gift box" style="cursor: pointer;" onclick="nextStep(7)">
        <p>Tap the gift to open it!</p>
    </div>

    <!-- STEP 7: Virtual Hug Grand Finale -->
    <div id="step7" class="card hidden">
        <h2>Here is a virtual hug for you 🤗</h2>
        <img class="gif-display" src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExbWwxdGg1ZzdicTJwNXg1M3gzMGxnd2dzYTM3dW5pdmluZTh0amxjOCZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9cw/9unqM66sC536G4DcoG/giphy.gif" alt="Cute mocha bear hug" style="width: 250px; height: 250px;">
        <p style="font-weight: bold; color: #d81b60;">I love you to the moon and back!</p>
    </div>

    <script>
        // Customization Configuration
        const CORRECT_PASSWORD = "love"; // Set your password here (lowercase recommended)

        function checkStep1() {
            const passwordEntered = document.getElementById('passwordInput').value.toLowerCase().trim();
            const captchaChecked = document.getElementById('captchaBox').checked;

            if (passwordEntered === CORRECT_PASSWORD && captchaChecked) {
                nextStep(2);
            } else if (passwordEntered !== CORRECT_PASSWORD) {
                alert("Incorrect Password! Try again.");
            } else {
                alert("Please confirm you are not a robot first!");
            }
        }

        function nextStep(stepNumber) {
            // Hide all cards
            document.querySelectorAll('.card').forEach(card => card.classList.add('hidden'));
            // Show the current step card
            document.getElementById('step' + stepNumber).classList.remove('hidden');
        }

        function tryClickNo() {
            // Take them to the angry dog screen if they choose 'No'
            document.querySelectorAll('.card').forEach(card => card.classList.add('hidden'));
            document.getElementById('stepAngry').classList.remove('hidden');
        }

        function backToQuestion() {
            nextStep(2);
        }
    </script>
</body>
</html>
