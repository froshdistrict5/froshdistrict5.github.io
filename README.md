<html lang="en">
<head>
  <title>District 5 — Frosh Week Hunger Games</title>
  <style>
    body {
      margin: 0;
      font-family: 'Orbitron', sans-serif;
      background: url("img.png") no-repeat center center fixed;
      background-size: cover;
      background-clip: border-box;
      -webkit-background-clip: border-box;
      color: #0ff;
      text-align: center;
      min-height: 100vh;
      display: flex;
      flex-direction: column;
    }
    header {
      padding: 2rem 1rem;
      background: linear-gradient(90deg, #0ff, #f0f, #ff0);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
      font-size: clamp(2rem, 6vw, 3.5rem);
      font-weight: bold;
      animation: flicker 2s infinite;
      line-height: 1.2;
    }
    @keyframes flicker {
      0%, 19%, 21%, 23%, 25%, 54%, 56%, 100% { opacity: 1; }
      20%, 24%, 55% { opacity: 0; }
    }
    section {
      margin: 1.5rem auto;
      max-width: 90%;
      padding: 1rem;
    }
    .card {
      background: rgba(0,0,0,0.6);
      border: 1px solid #0ff;
      border-radius: 12px;
      padding: 1rem;
      margin: 1rem 0;
      box-shadow: 0 0 20px #0ff5;
    }
    h2 {
      color: #ff0;
      font-size: clamp(1.2rem, 4vw, 2rem);
    }
    #countdown {
      font-size: clamp(1.2rem, 5vw, 2rem);
      margin-top: 1rem;
      color: #f0f;
    }
    input[type="text"] {
      width: 90%;
      max-width: 300px;
      padding: 0.5rem;
      border-radius: 6px;
      border: 1px solid #0ff;
      margin-top: 0.5rem;
    }
    button {
      background: #0ff;
      border: none;
      padding: 0.8rem 1.5rem;
      border-radius: 8px;
      font-size: 1rem;
      font-weight: bold;
      cursor: pointer;
      margin-top: 1rem;
      transition: transform 0.2s, background 0.3s;
    }
    button:hover {
      transform: scale(1.1);
      background: #0cc;
    }
    footer {
      margin-top: auto;
      padding: 1rem;
      font-size: 0.8rem;
      color: #ccc;
    }
  </style>
</head>
<body>
  <header>
    District 5 — Frosh Week Hunger Games ⚡️
  </header>

  <section>
    <div class="card">
      <h2>The Arena Opens In:</h2>
      <div id="countdown"></div>
    </div>
  </section>

  <section>
    <div class="card">
      <h2>Event Schedule</h2>
      <p>🏹 Day 1: Tribute Selection & Opening Ceremonies</p>
      <p>⚡ Day 2: Obstacle Course — Outrun Campus Security</p>
      <p>🔥 Day 3: Bonfire Night (Don’t get voted off the island by mistake)</p>
      <p>🥤 Day 4: Mocktail Mixer in the Capitol Lounge</p>
      <p>🏆 Day 5: Final Showdown & Closing Feast</p>
    </div>
  </section>

  <section>
    <div class="card">
      <h2>Register as Tribute</h2>
      <p>Think you have what it takes? Enter your name below and may the odds be ever in your favor.</p>
      <input type="text" id="tributeName" placeholder="Your Name">
      <br>
      <button onclick="registerTribute()">Enter Arena</button>
      <p id="tributeOutput"></p>
    </div>
  </section>

  <footer>
    Powered by District 5 Energy — Frosh Week 2025 ⚡️
  </footer>

  <script>
    // Countdown Timer
    const targetDate = new Date("2025-09-01T12:00:00").getTime();
    const countdownEl = document.getElementById("countdown");

    setInterval(() => {
      const now = new Date().getTime();
      const diff = targetDate - now;

      if (diff <= 0) {
        countdownEl.innerHTML = "The Games Have Begun!";
        return;
      }

      const days = Math.floor(diff / (1000 * 60 * 60 * 24));
      const hours = Math.floor((diff % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
      const minutes = Math.floor((diff % (1000 * 60 * 60)) / (1000 * 60));
      const seconds = Math.floor((diff % (1000 * 60)) / 1000);

      countdownEl.innerHTML = `${days}d ${hours}h ${minutes}m ${seconds}s`;
    }, 1000);

    // Tribute Registration
    function registerTribute() {
      const name = document.getElementById("tributeName").value.trim();
      const output = document.getElementById("tributeOutput");

      if (name) {
        output.innerHTML = `🎉 Welcome, Tribute <strong>${name}</strong>! The Capitol salutes you.`;
      } else {
        output.innerHTML = "Please enter a valid name, future Tribute.";
      }
    }
  </script>
</body>
</html>
