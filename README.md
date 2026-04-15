




<html lang="en">
<head>
<meta charset="UTF-8">
<title>UKWL X WLAN</title>
<style>
  body {
    margin: 0;
    height: 100vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    background: #050816;
    color: #fff;
    font-family: Arial, sans-serif;
  }

  h1 {
    font-size: 3rem;
    margin-bottom: 0.3rem;
    letter-spacing: 3px;
  }

  .subtitle {
    font-size: 1.1rem;
    opacity: 0.8;
    margin-bottom: 2rem;
  }

  /* CLOCK */
  .clock {
    width: 200px;
    height: 200px;
    border: 6px solid rgba(255,255,255,0.2);
    border-radius: 50%;
    position: relative;
    background: rgba(255,255,255,0.05);
    backdrop-filter: blur(10px);
  }

  .hand {
    position: absolute;
    width: 50%;
    height: 4px;
    background: white;
    top: 50%;
    transform-origin: 100%;
    transform: rotate(90deg);
    border-radius: 2px;
  }

  .hand.hour {
    height: 5px;
    width: 35%;
    background: #fff;
  }

  .hand.minute {
    height: 4px;
    width: 45%;
    background: #ddd;
  }

  .hand.second {
    height: 2px;
    width: 48%;
    background: #ff3b3b;
  }

  .center-dot {
    width: 12px;
    height: 12px;
    background: #ff3b3b;
    border-radius: 50%;
    position: absolute;
    top: calc(50% - 6px);
    left: calc(50% - 6px);
  }
</style>
</head>
<body>

<h1>UKWL X WLAN</h1>
<div class="subtitle">This page is being updated by WLAN Developers</div>

<div class="clock">
  <div class="hand hour" id="hourHand"></div>
  <div class="hand minute" id="minuteHand"></div>
  <div class="hand second" id="secondHand"></div>
  <div class="center-dot"></div>
</div>

<script>
  function updateClock() {
    const now = new Date();

    const seconds = now.getSeconds();
    const minutes = now.getMinutes();
    const hours = now.getHours();

    const secondDeg = seconds * 6; 
    const minuteDeg = minutes * 6 + seconds * 0.1;
    const hourDeg = (hours % 12) * 30 + minutes * 0.5;

    document.getElementById("secondHand").style.transform = `rotate(${secondDeg}deg)`;
    document.getElementById("minuteHand").style.transform = `rotate(${minuteDeg}deg)`;
    document.getElementById("hourHand").style.transform = `rotate(${hourDeg}deg)`;
  }

  setInterval(updateClock, 1000);
  updateClock();
</script>

</body>
</html>
