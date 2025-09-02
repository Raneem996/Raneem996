<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Raneem Portfolio</title>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Tajawal:wght@400;700&display=swap');

    body {
      margin: 0;
      padding: 0;
      background: linear-gradient(135deg, #6e8efb, #a777e3);
      font-family: 'Tajawal', sans-serif;
      color: #fff;
      text-align: center;
    }

    /* ===== Logo Section ===== */
    .logo-container {
      position: relative;
      text-align: center;
      perspective: 1000px;
      padding: 100px 20px 60px;
    }

    .logo {
      font-size: 4rem;
      font-weight: 700;
      color: #fff;
      text-shadow: 0 2px 10px rgba(0, 0, 0, 0.2);
      position: relative;
      display: inline-block;
    }

    .first-name, .second-name {
      display: inline-block;
      position: relative;
    }

    .first-name {
      color: #ff7e5f;
      animation: slideIn 2s ease-out, colorChangeFirst 6s infinite;
    }

    .second-name {
      color: #feb47b;
      animation: slideIn 2s ease-out 0.5s both, colorChangeSecond 6s infinite 1s;
    }

    .ampersand {
      display: inline-block;
      margin: 0 15px;
      opacity: 0;
      animation: fadeIn 1s ease-out 1.5s forwards;
      color: #fff;
      font-size: 3rem;
      transform: translateY(10px);
    }

    .decoration {
      position: absolute;
      border-radius: 50%;
      background: rgba(255, 255, 255, 0.1);
      animation: float 8s infinite ease-in-out;
    }

    .decoration:nth-child(1) {
      width: 80px;
      height: 80px;
      top: -40px;
      left: -40px;
      animation-delay: 0s;
    }

    .decoration:nth-child(2) {
      width: 40px;
      height: 40px;
      bottom: 20px;
      right: 50px;
      animation-delay: 1s;
    }

    .decoration:nth-child(3) {
      width: 60px;
      height: 60px;
      bottom: -30px;
      left: 50px;
      animation-delay: 2s;
    }

    @keyframes slideIn {
      from { opacity: 0; transform: translateY(50px) rotateX(90deg); }
      to { opacity: 1; transform: translateY(0) rotateX(0); }
    }

  
    
    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(10px); }
      to { opacity: 1; transform: translateY(0); }
    }

    @keyframes colorChangeFirst {
      0% { color: #ff7e5f; }
      50% { color: #ffcc67; }
      100% { color: #ff7e5f; }
    }

    @keyframes colorChangeSecond {
      0% { color: #feb47b; }
      50% { color: #6adaff; }
      100% { color: #feb47b; }
    }

    @keyframes float {
      0%, 100% { transform: translateY(0) scale(1); }
      50% { transform: translateY(-20px) scale(1.05); }
    }

    /* ===== Bio Section ===== */
    section {
      max-width: 900px;
      margin: 0 auto;
      padding: 40px 20px;
      background: rgba(255, 255, 255, 0.1);
      border-radius: 20px;
      margin-bottom: 40px;
    }

    h1, h2 {
      color: #fff;
    }

    ul {
      list-style: none;
      padding: 0;
      font-size: 1.2rem;
    }

    ul li {
      margin: 10px 0;
    }

    img {
      max-width: 100%;
    }
  </style>
</head>
<body>
  <!-- Logo Section -->
  <div class="logo-container">
    <div class="decoration"></div>
    <div class="decoration"></div>
    <div class="decoration"></div>
    
    <div class="logo">
      <span class="first-name">Raneem</span>
      <span class="ampersand">&</span>
      <span class="second-name">Mohsen</span>
    </div>
  </div>

  <!-- Bio Section -->
  <section>
    <h1 align="center">👋 Hi, I'm Raneem ^_^ </h1>
    <p align="center">
      I am <strong>Raneem Mohsen</strong>, a developer interested in <strong>Data Analysis</strong> and <strong>Artificial Intelligence</strong>.  
      I aim to improve my programming skills and build practical projects using modern tools.
    </p>
  </section>

  <!-- Skills -->
  <section>
    <h2>🧰 Skills & Interests</h2>
    <ul>
      <li>📊 Data Analysis</li>
      <li>🤖 Artificial Intelligence (AI)</li>
      <li>☕ Java (OOP)</li>
      <li>🐍 Python (Pandas, NumPy, Matplotlib)</li>
      <li>📈 Machine Learning</li>
      <li>🌐 Git & GitHub for collaboration and projects</li>
    </ul>
  </section>

  <!-- GitHub Stats -->
  <section>
    <h2>📊 GitHub Stats</h2>
    <p align="center">
      <img src="https://github-readme-stats.vercel.app/api?username=Raneem996&show_icons=true&hide_title=true" alt="GitHub Stats" />
      <br />
      <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Raneem996&layout=compact" alt="Top Languages" />
    </p>
  </section>

  <script>
    // تغيير الاسم بسهولة
    document.querySelector('.first-name').textContent = 'Raneem';
    document.querySelector('.second-name').textContent = 'Mohsen';

    // تأثير حركة مع الماوس
    document.addEventListener('mousemove', (e) => {
      const x = (window.innerWidth / 2 - e.pageX) / 25;
      const y = (window.innerHeight / 2 - e.pageY) / 25;
      document.querySelector('.logo-container').style.transform = `translate(${x}px, ${y}px)`;
    });
  </script>
</body>
</html>


