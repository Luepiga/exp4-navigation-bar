<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>GlowApp | Welcome</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <style>
    html {
      scroll-behavior: smooth;
    }

    body, html {
      height: 100%;
      font-family: 'Poppins', Arial, sans-serif;
      margin: 0;
      padding: 0;
      background: linear-gradient(135deg,#6d5bba 0%,#8d58bf 100%);
      min-height: 100vh;
    }

    .navbar {
      position: fixed;
      top: 0;
      width: 100%;
      background: rgba(20,20,40,0.6);
      backdrop-filter: blur(10px);
      box-shadow: 0 8px 20px rgba(0,0,0,0.1);
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 12px 30px;
      z-index: 999;
    }

    .logo {
      display: flex;
      align-items: center;
      gap: 10px;
    }

    .logo img {
      height: 42px;
      border-radius: 12px;
      box-shadow: 0 2px 12px #0004;
    }

    .logo span {
      color: #fff;
      font-size: 26px;
      font-weight: 700;
      letter-spacing: 1px;
      text-shadow: 0 1px 4px #333;
    }

    .nav-links {
      display: flex;
      list-style: none;
      gap: 30px;
    }

    .nav-links a {
      color: #f3f1ff;
      font-size: 110%;
      text-decoration: none;
      padding: 7px 15px;
      border-radius: 20px;
      transition: background 0.2s, color 0.25s;
    }

    .nav-links a:hover, .nav-links a:focus {
      background: rgba(150,120,255,0.18);
      color: #00fff7;
      outline: none;
    }

    section {
      padding: 100px 30px;
      color: white;
      text-align: center;
    }

    .landing {
      background: url('c:\\Users\\URK23CS1083\\Downloads\\512x512bb.jpg') center/cover no-repeat;
      position: relative;
    }

    .overlay {
      position: absolute;
      width: 100%;
      height: 100%;
      left: 0; top: 0;
      background: rgba(30,0,50,0.42);
      z-index: 0;
    }

    .login-container {
      position: relative;
      z-index: 2;
      width: 370px;
      margin: auto;
      border-radius: 18px;
      background: rgba(255,255,255,0.19);
      box-shadow: 0 8px 42px 0 rgba(68,28,207,0.19), 0 1.5px 8px rgba(17,12,46,0.15);
      padding: 42px 35px;
      backdrop-filter: blur(13px);
      border: 1px solid rgba(255,255,255,0.16);
      margin-top: 120px;
    }

    .login-container h2 {
      text-align: center;
      color: #fff;
      font-size: 1.6rem;
      margin-bottom: 22px;
    }

    .login-form {
      display: grid;
      gap: 18px;
    }

    .login-form input,
    .login-form button {
      padding: 11px 14px;
      border-radius: 8px;
      border: none;
      font-size: 1em;
      outline: none;
    }

    .login-form input {
      background: rgba(252,251,255,0.65);
      color: #2d2c4c;
    }

    .login-form input:focus {
      box-shadow: 0 0 0 3px #6f99ff44;
    }

    .login-form button {
      background: linear-gradient(90deg,#7b63fa 20%,#1de9b6 80%);
      color: #fff;
      font-weight: bold;
      cursor: pointer;
      transition: all 0.3s ease;
    }

    .login-form button:hover {
      background: linear-gradient(90deg,#1de9b6,#7b63fa 98%);
      transform: scale(1.03);
    }

  
    #home {
      background-color: #6d5bba;
    }

    #features {
      background-color: #5c4ba1;
    }

    #pricing {
      background-color: #4a398a;
    }

    #contact {
      background-color: #392871;
    }

    h2.section-title {
      font-size: 2.4rem;
      margin-bottom: 20px;
    }

    p.section-text {
      font-size: 1.1rem;
      max-width: 700px;
      margin: 0 auto;
      line-height: 1.7;
    }

    @media (max-width: 600px) {
      .login-container {
        width: 90%;
        padding: 30px;
      }

      .nav-links {
        flex-direction: column;
        gap: 10px;
      }

      .navbar {
        flex-direction: column;
        align-items: flex-start;
        padding: 15px;
      }
    }
  </style>
</head>
<body>


<header class="navbar">
  <div class="logo">
    <img src="https://cdn-icons-png.flaticon.com/512/3566/3566336.png" alt="GlowApp Logo" />
    <span>GlowApp</span>
  </div>
  <nav>
    <ul class="nav-links">
      <li><a href="#home">Home</a></li>
      <li><a href="#features">Features</a></li>
      <li><a href="#pricing">Pricing</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>
</header>


<section id="home" class="landing">
  <div class="overlay"></div>
  <div class="login-container">
    <h2>Sign in to GlowApp</h2>
    <form class="login-form">
      <input type="email" placeholder="Email" required />
      <input type="password" placeholder="Password" required />
      <button type="submit">Login</button>
    </form>
  </div>
</section>


<section id="features">
  <h2 class="section-title">Features</h2>
  <p class="section-text">
    GlowApp offers real-time collaboration, data-sync across devices, AI-powered intelligence, and a customizable dashboard to supercharge your productivity.
  </p>
</section>


<section id="pricing">
  <h2 class="section-title">Pricing</h2>
  <p class="section-text">
    Choose from our flexible pricing: Free Basic Plan for individuals, Pro Plan at $9.99/month for professionals, and Business Plan for teams starting at $24.99/month.
  </p>
</section>


<section id="contact">
  <h2 class="section-title">Contact Us</h2>
  <p class="section-text">
    Have questions or suggestions? Reach out to us at <strong>support@glowapp.io</strong>, or visit our HQ in Pune, India. We’re happy to help!
  </p>
</section>

</body>
</html>
