




<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>WLAN X UKWL | Blacklist</title>

    <style>
        /* Fade‑in animation */
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }

        body {
            margin: 0;
            padding: 0;
            background: #0b0b0b;
            font-family: Arial, sans-serif;
            color: white;
            text-align: center;
            animation: fadeIn 1s ease-out;
        }

        /* Title glow + exact weight */
        .title {
            font-size: 70px;
            font-weight: 900;
            margin-top: 70px;
            color: #ff4dd2;
            text-shadow: 0 0 15px #ff4dd2, 0 0 30px #ff1ab8;
            letter-spacing: 3px;
            animation: fadeIn 1.2s ease-out;
        }

        .subtitle {
            font-size: 38px;
            font-weight: 700;
            margin-top: -10px;
            color: #ffffff;
            animation: fadeIn 1.4s ease-out;
        }

        .description {
            margin-top: 8px;
            font-size: 16px;
            color: #cccccc;
            animation: fadeIn 1.6s ease-out;
        }

        /* Section headers */
        .section-header {
            margin-top: 60px;
            font-size: 28px;
            font-weight: 800;
            text-decoration: underline;
            animation: fadeIn 1.8s ease-out;
        }

        /* Card styling */
        .card {
            width: 55%;
            margin: 25px auto;
            background: #141414;
            padding: 25px;
            border-radius: 12px;
            border: 1px solid #2a2a2a;
            text-align: left;
            box-shadow: 0 0 15px rgba(255, 77, 210, 0.15);
            animation: fadeIn 2s ease-out;
        }

        .label {
            font-weight: 700;
            color: #ff4dd2;
        }

        .copy-btn {
            float: right;
            background: #ff4dd2;
            border: none;
            padding: 7px 14px;
            border-radius: 6px;
            cursor: pointer;
            color: black;
            font-weight: 700;
            transition: 0.2s;
        }

        .copy-btn:hover {
            background: #ff1ab8;
        }

        span[contenteditable="true"] {
            color: #e6e6e6;
            font-weight: 500;
        }
    </style>

    <script>
        function copyText(id) {
            const text = document.getElementById(id).innerText;
            navigator.clipboard.writeText(text);
        }
    </script>
</head>

<body>

    <div class="title">WLAN X UKWL</div>
    <div class="subtitle">Blacklist Database</div>
    <div class="description">
        This is the official page where all blacklist information will be shown for UK West London Roleplay.
    </div>

    <!-- USER BLACKLIST -->
    <div class="section-header">USER BLACKLIST</div>

    <div class="card">
        <button class="copy-btn" onclick="copyText('user1')">Copy</button>
        <div id="user1">
            <span class="label">Username:</span> <span contenteditable="true">supervisor.563_</span><br><br>
            <span class="label">User ID:</span> <span contenteditable="true">1249004934503071827</span><br><br>
            <span class="label">Roblox User:</span> <span contenteditable="true">axel_king223</span><br><br>
            <span class="label">Roblox ID:</span> <span contenteditable="true">3022169889</span><br><br>
            <span class="label">Reason:</span> <span contenteditable="true">Coping Assets, harassment, endangerment of other users & Raiding servers.</span><br><br>
            <span class="label">Evidence:</span> <span contenteditable="true">https://docs.google.com/document/d/10ri45eE2n7H4KIniNLBbLV-DJpKZFyp4lk71s4AEHBE/edit?usp=sharing</span>
        </div>
    </div>

    <!-- SERVER BLACKLIST -->
    <div class="section-header">SERVER BLACKLIST</div>

    <div class="card">
        <button class="copy-btn" onclick="copyText('server1')">Copy</button>
        <div id="server1">
            <span class="label">Server Name:</span> <span contenteditable="true">Florida State Roleplay </span><br><br>
            <span class="label">Server ID:</span> <span contenteditable="true">1476035069822107728</span><br><br>
            <span class="label">Owner Username:</span> <span contenteditable="true">supervisor.563_</span><br><br>
            <span class="label">Owner ID:</span> <span contenteditable="true">1249004934503071827</span><br><br>
            <span class="label">Reason:</span> <span contenteditable="true">The owner is blacklisted.</span><br><br>
            <span class="label">Evidence:</span> <span contenteditable="true">https://docs.google.com/document/d/10ri45eE2n7H4KIniNLBbLV-DJpKZFyp4lk71s4AEHBE/edit?usp=sharing</span>
        </div>
    </div>

</body>
</html>
