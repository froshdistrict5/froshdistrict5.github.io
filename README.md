
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>District 5 — Frosh Week Hunger Games</title>
  <style>
    /* Base styles */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: "Trebuchet MS", sans-serif;
      color: white;
      text-align: center;
      min-height: 100vh;
      background: url("A_promotional_digital_image_for_\"District_5_–_Powe.png") no-repeat center center fixed;
      background-size: cover;
      background-clip: border-box;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      animation: fadeIn 2s ease-in-out;
    }

    h1 {
      font-size: 3rem;
      text-shadow: 2px 2px 6px black;
      margin-bottom: 1rem;
      animation: glow 2s infinite alternate;
    }

    h2 {
      font-size: 1.5rem;
      margin-bottom: 2rem;
      text-shadow: 1px 1px 5px black;
    }

    p {
      font-size: 1.2rem;
      max-width: 600px;
      margin: auto;
      margin-bottom: 1.5rem;
      text-shadow: 1px 1px 5px black;
    }

    .btn {
      display: inline-block;
      padding: 12px 25px;
      margin: 10px;
      border: 2px solid white;
      border-radius: 12px;
      text-decoration: none;
      color: white;
      font-size: 1.2rem;
      transition: all 0.3s ease;
      backdrop-filter: blur(5px);
    }

    .btn:hover {
      background: rgba(255, 255, 255, 0.2);
      transform: scale(1.1);
      box-shadow: 0 0 15px #ffde59;
    }

    .card-container {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 20px;
      width: 90%;
      margin: 40px auto;
    }

    .card {
      background: rgba(0, 0, 0, 0.6);
      border-radius: 15px;
      padding: 20px;
      text-align: center;
      transition: transform 0.3s ease, box-shadow 0.3s ease;
      backdrop-filter: blur(8px);
    }

    .card:hover {
      transform: translateY(-10px);
      box-shadow: 0 0 20px #ffde59;
    }

    footer {
      margin-top: 50px;
      font-size: 0.9rem;
      text-shadow: 1px 1px 5px black;
    }

    /* Animations */
    @keyframes fadeIn {
      from { opacity: 0; }
      to { opacity: 1; }
    }

    @keyframes glow {
      from { text-shadow: 2px 2px 10px #ffde59; }
      to { text-shadow: 2px 2px 20px #ffffff; }
    }

    /* Mobile Friendly */
    @media (max-width: 768px) {
      h1 { font-size: 2rem; }
      h2 { font-size: 1.2rem; }
      p { font-size: 1rem; }
      .btn { font-size: 1rem; padding: 10px 18px; }
    }
  </style>
</head>
<body>
  <h1>🔥 District 5 — Frosh Week 🔥</h1>
  <h2>"The Powerhouse of the Games ⚡"</h2>
  <p>Welcome, tributes of District 5! You don’t just survive Frosh Week — you thrive with ENERGY. May the odds be ever in your favour (unless you forget your student card).</p>

  <a href="#" class="btn">Join the Rebellion</a>
  <a href="#" class="btn">Charge Your Spirit</a>

  <div class="card-container">
    <div class="card">
      <h3>⚡ Power Games</h3>
      <p>Compete in high-voltage challenges — caffeine-fueled dodgeball, late-night trivia, and more!</p>
    </div>
    <div class="card">
      <h3>🎉 Nightlife</h3>
      <p>Dance like you’re rebelling against the Capitol. Glow sticks = mandatory.</p>
    </div>
    <div class="card">
      <h3>🍕 Survival Rations</h3>
      <p>Pizza is our bread and circuses. Eat like Katniss after a victory tour.</p>
    </div>
  </div>

  <footer>
    &copy; 2025 District 5 Frosh Week | Powered by ENERGY ⚡
  </footer>
</body>
</html>
