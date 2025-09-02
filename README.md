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


