<!DOCTYPE html>
<html lang="ka">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Car Detailing • Studio & Mobile Service</title>

  <!-- Google Fonts -->
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;600;700&family=Inter:wght@300;400;500&display=swap" rel="stylesheet">

  <style>
    :root {
      --bg-dark: #0f1115;
      --bg-light: #161a22;
      --text-main: #ffffff;
      --text-muted: #a0a4ad;
      --accent: #1e90ff;
      --card-bg: #1b1f2a;
    }

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Inter', sans-serif;
      background: var(--bg-dark);
      color: var(--text-main);
      line-height: 1.6;
    }

    a {
      color: inherit;
      text-decoration: none;
    }

    /* HEADER */
    header {
      padding: 20px 40px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      position: sticky;
      top: 0;
      background: rgba(15,17,21,0.9);
      backdrop-filter: blur(8px);
      z-index: 100;
    }

    .logo {
      font-family: 'Montserrat', sans-serif;
      font-size: 22px;
      font-weight: 700;
    }

    nav a {
      margin-left: 24px;
      font-size: 14px;
      color: var(--text-muted);
    }

    nav a:hover {
      color: var(--text-main);
    }

    /* HERO */
    .hero {
      min-height: 90vh;
      display: flex;
      align-items: center;
      padding: 80px 40px;
      background: linear-gradient(rgba(0,0,0,0.6), rgba(0,0,0,0.6)), url('hero-car.jpg') center/cover no-repeat;
    }

    .hero-content {
      max-width: 600px;
    }

    .hero h1 {
      font-family: 'Montserrat', sans-serif;
      font-size: 46px;
      margin-bottom: 20px;
    }

    .hero p {
      color: var(--text-muted);
      margin-bottom: 32px;
      font-size: 18px;
    }

    .btn {
      display: inline-block;
      padding: 14px 28px;
      background: var(--accent);
      color: #fff;
      border-radius: 6px;
      font-weight: 600;
      margin-right: 12px;
    }

    .btn.secondary {
      background: transparent;
      border: 1px solid var(--accent);
    }

    /* SECTIONS */
    section {
      padding: 80px 40px;
    }

    .section-title {
      font-family: 'Montserrat', sans-serif;
      font-size: 32px;
      margin-bottom: 40px;
      text-align: center;
    }

    /* FEATURES */
    .features {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
      gap: 24px;
    }

    .feature-card {
      background: var(--card-bg);
      padding: 32px;
      border-radius: 10px;
      text-align: center;
    }

    /* SERVICES */
    .services {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 24px;
    }

    .service-card {
      background: var(--card-bg);
      padding: 28px;
      border-radius: 10px;
    }

    .service-card h3 {
      margin-bottom: 12px;
      font-family: 'Montserrat', sans-serif;
    }

    /* HOW IT WORKS */
    .steps {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
      gap: 24px;
      text-align: center;
    }

    .step {
      background: var(--card-bg);
      padding: 24px;
      border-radius: 10px;
    }

    /* FOOTER */
    footer {
      padding: 40px;
      background: var(--bg-light);
      text-align: center;
      font-size: 14px;
      color: var(--text-muted);
    }

    /* MOBILE */
    @media (max-width: 768px) {
      .hero h1 {
        font-size: 34px;
      }

      nav {
        display: none;
      }
    }
  </style>
</head>
<body>

<header>
  <div class="logo">DETAILING PRO</div>
  <nav>
    <a href="#services">სერვისები</a>
    <a href="#mobile">გამოძახება</a>
    <a href="#contact">კონტაქტი</a>
  </nav>
</header>

<section class="hero">
  <div class="hero-content">
    <h1>პროფესიონალური Car Detailing<br>სტუდიაში ან შენთან ადგილზე</h1>
    <p>დაზოგე დრო — ჩვენ მოვალთ სრულად აღჭურვილი და დაგიბრუნებთ იდეალურად სუფთა მანქანას.</p>
    <a href="#contact" class="btn">დაჯავშნე გამოძახება</a>
    <a href="#services" class="btn secondary">იხილე სერვისები</a>
  </div>
</section>

<section>
  <h2 class="section-title">რატომ ჩვენ?</h2>
  <div class="features">
    <div class="feature-card">🚐 ადგილზე მომსახურება</div>
    <div class="feature-card">🧼 პრემიუმ მასალები</div>
    <div class="feature-card">⏱ სწრაფი სერვისი</div>
    <div class="feature-card">⭐ გარანტირებული ხარისხი</div>
  </div>
</section>

<section id="services">
  <h2 class="section-title">სერვისები</h2>
  <div class="services">
    <div class="service-card"><h3>Exterior Detailing</h3><p>გარეცხვისა და დაცვითი პროცედურები.</p></div>
    <div class="service-card"><h3>Interior Detailing</h3><p>სალონის ღრმა წმენდა.</p></div>
    <div class="service-card"><h3>Ceramic Coating</h3><p>გრძელვადიანი დაცვა.</p></div>
    <div class="service-card"><h3>Mobile Detailing</h3><p>გამოძახებით, შენს ლოკაციაზე.</p></div>
  </div>
</section>

<section id="mobile">
  <h2 class="section-title">როგორ მუშაობს გამოძახება</h2>
  <div class="steps">
    <div class="step">1. ირჩევ სერვისს</div>
    <div class="step">2. უთითებ ლოკაციას</div>
    <div class="step">3. მოვდივართ აღჭურვილობით</div>
    <div class="step">4. იღებ სუფთა მანქანას</div>
  </div>
</section>

<footer id="contact">
  <p>📞 +995 XXX XX XX XX | 💬 WhatsApp</p>
  <p>© 2026 Detailing Pro. All rights reserved.</p>
</footer>

</body>
</html>
