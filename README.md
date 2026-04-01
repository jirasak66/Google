<!DOCTYPE html>
<html lang="th">
<head>
  <meta charset="UTF-8">
  <title>My Beautiful Website</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <!-- Google Font -->
  <link href="https://fonts.googleapis.com/css2?family=Prompt:wght@300;500;700&display=swap" rel="stylesheet">

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Prompt', sans-serif;
    }

    body {
      background: linear-gradient(135deg, #1e3c72, #2a5298);
      color: white;
      scroll-behavior: smooth;
    }

    header {
      display: flex;
      justify-content: space-between;
      padding: 20px 50px;
      background: rgba(0,0,0,0.3);
      position: fixed;
      width: 100%;
      backdrop-filter: blur(10px);
    }

    header h1 {
      font-weight: 700;
    }

    nav a {
      color: white;
      text-decoration: none;
      margin-left: 20px;
      transition: 0.3s;
    }

    nav a:hover {
      color: #00eaff;
    }

    .hero {
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      flex-direction: column;
      text-align: center;
      animation: fadeIn 2s ease;
    }

    .hero h2 {
      font-size: 48px;
      margin-bottom: 10px;
    }

    .hero p {
      font-size: 20px;
      opacity: 0.8;
    }

    .btn {
      margin-top: 20px;
      padding: 12px 25px;
      border: none;
      border-radius: 30px;
      background: #00eaff;
      color: black;
      cursor: pointer;
      font-weight: bold;
      transition: 0.3s;
    }

    .btn:hover {
      transform: scale(1.1);
      background: #00c2cc;
    }

    section {
      padding: 80px 50px;
      text-align: center;
    }

    .cards {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
      margin-top: 30px;
    }

    .card {
      background: rgba(255,255,255,0.1);
      padding: 30px;
      border-radius: 20px;
      backdrop-filter: blur(10px);
      transition: 0.3s;
    }

    .card:hover {
      transform: translateY(-10px);
      background: rgba(255,255,255,0.2);
    }

    footer {
      text-align: center;
      padding: 20px;
      background: rgba(0,0,0,0.3);
    }

    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(30px); }
      to { opacity: 1; transform: translateY(0); }
    }
  </style>
</head>

<body>

<header>
  <h1>MySite</h1>
  <nav>
    <a href="#">Home</a>
    <a href="#about">About</a>
    <a href="#services">Services</a>
  </nav>
</header>

<div class="hero">
  <h2>ยินดีต้อนรับสู่เว็บไซต์ของคุณ</h2>
  <p>สวย เท่ ทันสมัย ด้วย HTML + CSS</p>
  <button class="btn" onclick="showMessage()">เริ่มต้น</button>
</div>

<section id="about">
  <h2>เกี่ยวกับเรา</h2>
  <p>เว็บไซต์นี้ถูกออกแบบให้ดูทันสมัย รองรับมือถือ และใช้งานง่าย</p>
</section>

<section id="services">
  <h2>บริการของเรา</h2>
  <div class="cards">
    <div class="card">💻 Web Design</div>
    <div class="card">📱 Mobile Friendly</div>
    <div class="card">⚡ Fast Performance</div>
  </div>
</section>

<footer>
  <p>© 2026 My Beautiful Website</p>
</footer>

<script>
  function showMessage() {
    alert("เริ่มใช้งานเว็บไซต์แล้ว!");
  }
</script>

</body>
</html>
