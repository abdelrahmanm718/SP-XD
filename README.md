<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Abdelrahman Medhat | Portfolio</title>
  <style>
    /* ========== Reset ========== */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    }

    body {
      background: linear-gradient(135deg, #0f172a, #1e293b);
      color: white;
      display: flex;
      justify-content: center;
      align-items: center;
      min-height: 100vh;
    }

    .card {
      background: rgba(255, 255, 255, 0.05);
      backdrop-filter: blur(10px);
      padding: 30px;
      border-radius: 20px;
      text-align: center;
      max-width: 400px;
      width: 90%;
      box-shadow: 0 0 20px rgba(0,0,0,0.3);
      animation: fadeIn 1.2s ease;
    }

    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(30px);}
      to { opacity: 1; transform: translateY(0);}
    }

    .card img {
      width: 120px;
      height: 120px;
      border-radius: 50%;
      object-fit: cover;
      border: 3px solid #38bdf8;
      margin-bottom: 15px;
    }

    h1 {
      font-size: 1.8rem;
      margin-bottom: 8px;
    }

    p.bio {
      font-size: 0.95rem;
      opacity: 0.85;
      margin-bottom: 20px;
    }

    .section {
      margin-bottom: 20px;
      text-align: left;
    }

    .section h2 {
      font-size: 1.1rem;
      margin-bottom: 10px;
      color: #38bdf8;
    }

    .skills span {
      display: inline-block;
      background: #38bdf8;
      color: #0f172a;
      padding: 6px 12px;
      border-radius: 15px;
      margin: 5px 5px 0 0;
      font-size: 0.85rem;
      font-weight: 600;
    }

    .goals p {
      font-size: 0.9rem;
      opacity: 0.9;
      line-height: 1.4;
    }

    .social a {
      display: inline-block;
      margin: 0 10px;
      color: #38bdf8;
      text-decoration: none;
      font-size: 1.5rem;
      transition: 0.3s;
    }

    .social a:hover {
      color: #0ea5e9;
      transform: scale(1.1);
    }

    .view-counter {
      margin-top: 20px;
      font-size: 0.9rem;
      opacity: 0.8;
    }

    /* ========== Responsive ========== */
    @media (max-width: 480px) {
      h1 { font-size: 1.5rem; }
      .card img { width: 100px; height: 100px; }
    }
  </style>
</head>
<body>
  <div class="card">
    <img src="https://via.placeholder.com/150" alt="Profile Picture">
    <h1>Abdelrahman Medhat</h1>
    <p class="bio">I’m a passionate learner and content creator. I love sharing knowledge and building my personal brand through tech.</p>

    <div class="section skills">
      <h2>🛠 Skills</h2>
      <span>Python</span>
      <span>HTML</span>
      <span>CSS</span>
    </div>

    <div class="section goals">
      <h2>🚀 Interests & Goals</h2>
      <p>Front-End Development, Freelancing, and Building a strong personal brand to inspire others.</p>
    </div>

    <div class="section social">
      <h2>🌐 Connect</h2>
      <a href="http://www.youtube.com/@AMSEduCode" target="_blank" title="YouTube">
        📺
      </a>
    </div>

    <div class="view-counter">
      👀 Profile Views: <span id="views">0</span>
    </div>
  </div>

  <script>
    // Simple View Counter (local)
    let views = localStorage.getItem('profileViews') || 0;
    views++;
    localStorage.setItem('profileViews', views);
    document.getElementById('views').textContent = views;
  </script>
</body>
</html>


