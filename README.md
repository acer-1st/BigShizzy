<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <title>Big Shizzy | Artist & Entertainer</title>

  <meta
    name="description"
    content="Official website of Big Shizzy — artist, entertainer and creative professional from Ogun State, Nigeria."
  >

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    html {
      scroll-behavior: smooth;
    }

    body {
      font-family: Arial, Helvetica, sans-serif;
      background: #050505;
      color: #fff;
      line-height: 1.6;
      overflow-x: hidden;
    }

    :root {
      --black: #050505;
      --dark: #0c0c0c;
      --gold: #d4af37;
      --light-gold: #f4d675;
      --white: #fff;
      --gray: #aaa;
      --card: #111;
    }

    a {
      color: inherit;
      text-decoration: none;
    }

    img {
      max-width: 100%;
      display: block;
    }

    /* =========================
       HEADER
    ========================= */

    header {
      position: sticky;
      top: 0;
      z-index: 1000;
      background: rgba(5, 5, 5, 0.95);
      backdrop-filter: blur(12px);
      border-bottom: 1px solid rgba(212, 175, 55, 0.2);
    }

    .nav {
      width: 92%;
      max-width: 1200px;
      margin: auto;
      min-height: 75px;

      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 30px;
    }

    .logo {
      font-size: 24px;
      font-weight: 900;
      letter-spacing: 2px;
      color: var(--gold);
      white-space: nowrap;
    }

    .logo span {
      color: #fff;
    }

    nav {
      display: flex;
      align-items: center;
      gap: 28px;
    }

    nav a {
      color: #ddd;
      font-size: 14px;
      transition: 0.3s ease;
    }

    nav a:hover {
      color: var(--gold);
    }

    .nav-book {
      padding: 11px 18px;
      border: 1px solid var(--gold);
      border-radius: 30px;
      color: var(--gold) !important;
    }

    .nav-book:hover {
      background: var(--gold);
      color: #000 !important;
    }

    /* =========================
       HERO
    ========================= */

    .hero {
      min-height: calc(100vh - 75px);
      width: 92%;
      max-width: 1200px;
      margin: auto;

      display: grid;
      grid-template-columns: 1.1fr 0.9fr;
      align-items: center;
      gap: 70px;

      padding: 80px 0;
      position: relative;
    }

    .hero-content {
      position: relative;
      z-index: 2;
    }

    .eyebrow {
      display: inline-block;
      color: var(--gold);
      font-size: 13px;
      font-weight: bold;
      letter-spacing: 4px;
      margin-bottom: 18px;
      text-transform: uppercase;
    }

    .hero h1 {
      font-size: clamp(55px, 9vw, 110px);
      line-height: 0.9;
      text-transform: uppercase;
      letter-spacing: -5px;
      margin-bottom: 25px;
    }

    .hero h1 span {
      color: var(--gold);
    }

    .hero-description {
      max-width: 600px;
      color: var(--gray);
      font-size: 18px;
      margin-bottom: 32px;
    }

    .buttons {
      display: flex;
      flex-wrap: wrap;
      gap: 15px;
    }

    .btn {
      display: inline-flex;
      align-items: center;
      justify-content: center;

      padding: 14px 24px;
      border-radius: 4px;

      font-weight: bold;
      font-size: 14px;

      transition: 0.3s ease;
    }

    .btn-gold {
      background: var(--gold);
      color: #000;
    }

    .btn-gold:hover {
      background: var(--light-gold);
      transform: translateY(-3px);
      box-shadow: 0 10px 30px rgba(212, 175, 55, 0.25);
    }

    .btn-outline {
      border: 1px solid #555;
      color: #fff;
    }

    .btn-outline:hover {
      border-color: var(--gold);
      color: var(--gold);
      transform: translateY(-3px);
    }

    /* HERO IMAGE */

    .hero-image {
      position: relative;
      min-height: 560px;
      display: flex;
      justify-content: center;
      align-items: center;
    }

    .hero-image::before {
      content: "";
      position: absolute;
      width: 430px;
      height: 430px;
      border-radius: 50%;
      border: 1px solid rgba(212, 175, 55, 0.5);
      animation: rotate 15s linear infinite;
    }

    .hero-image::after {
      content: "";
      position: absolute;
      width: 500px;
      height: 500px;
      border-radius: 50%;
      background: radial-gradient(
        circle,
        rgba(212, 175, 55, 0.18),
        transparent 65%
      );
      animation: glow 3s ease-in-out infinite;
    }

    .hero-image img {
      width: min(100%, 440px);
      height: 550px;
      object-fit: cover;
      object-position: center;
      border-radius: 8px;
      position: relative;
      z-index: 2;

      border: 1px solid rgba(212, 175, 55, 0.45);

      box-shadow:
        0 0 40px rgba(212, 175, 55, 0.15),
        0 30px 80px rgba(0, 0, 0, 0.8);
    }

    /* =========================
       GENERAL
    ========================= */

    section {
      width: 92%;
      max-width: 1200px;
      margin: auto;
      padding: 110px 0;
    }

    .section-heading {
      margin-bottom: 55px;
    }

    .section-heading small {
      color: var(--gold);
      letter-spacing: 4px;
      text-transform: uppercase;
      font-weight: bold;
    }

    .section-heading h2 {
      font-size: clamp(38px, 6vw, 70px);
      line-height: 1;
      margin-top: 12px;
    }

    .section-heading p {
      color: var(--gray);
      max-width: 650px;
      margin-top: 18px;
    }

    /* =========================
       ABOUT PREVIEW
    ========================= */

    .about {
      background: var(--dark);
      width: 100%;
    }

    .about-inner {
      width: 92%;
      max-width: 1200px;
      margin: auto;

      display: grid;
      grid-template-columns: 0.8fr 1.2fr;
      gap: 70px;
      align-items: center;
    }

    .about-image {
      position: relative;
    }

    .about-image img {
      width: 100%;
      max-width: 430px;
      height: 520px;
      object-fit: cover;
      border-radius: 6px;
      border: 1px solid rgba(212, 175, 55, 0.4);
    }

    .about-content small {
      color: var(--gold);
      text-transform: uppercase;
      letter-spacing: 4px;
      font-weight: bold;
    }

    .about-content h2 {
      font-size: clamp(40px, 6vw, 68px);
      line-height: 1;
      margin: 12px 0 25px;
    }

    .about-content p {
      color: var(--gray);
      margin-bottom: 18px;
    }

    .about-link {
      display: inline-flex;
      margin-top: 15px;
      padding: 14px 23px;
      border: 1px solid var(--gold);
      color: var(--gold);
      font-weight: bold;
      transition: 0.3s ease;
    }

    .about-link:hover {
      background: var(--gold);
      color: #000;
      transform: translateY(-3px);
    }

    .facts {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      gap: 14px;
      margin: 30px 0;
    }

    .fact {
      background: #151515;
      padding: 17px;
      border-left: 2px solid var(--gold);
    }

    .fact strong {
      display: block;
      color: #fff;
      margin-bottom: 4px;
    }

    .fact span {
      color: var(--gray);
      font-size: 14px;
    }

    /* =========================
       SERVICES
    ========================= */

    .services-grid {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 16px;
    }

    .service-card {
      background: var(--card);
      padding: 30px 22px;
      min-height: 180px;

      border: 1px solid #222;
      transition: 0.35s ease;
      position: relative;
      overflow: hidden;
    }

    .service-card::after {
      content: "";
      position: absolute;
      width: 80px;
      height: 80px;
      background: rgba(212, 175, 55, 0.07);
      border-radius: 50%;
      right: -30px;
      bottom: -30px;
      transition: 0.35s ease;
    }

    .service-card:hover {
      transform: translateY(-7px);
      border-color: var(--gold);
    }

    .service-card:hover::after {
      transform: scale(2);
    }

    .service-number {
      color: var(--gold);
      font-size: 13px;
      font-weight: bold;
    }

    .service-card h3 {
      margin-top: 25px;
      font-size: 19px;
    }

    /* =========================
       MEDIA
    ========================= */

    .media {
      background: var(--dark);
      width: 100%;
    }

    .media-inner {
      width: 92%;
      max-width: 1200px;
      margin: auto;
    }

    .media-grid {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      gap: 25px;
    }

    .media-card {
      position: relative;
      overflow: hidden;
      background: #111;
      border: 1px solid #222;
    }

    .media-card img {
      width: 100%;
      height: 500px;
      object-fit: cover;
      transition: 0.5s ease;
    }

    .media-card:hover img {
      transform: scale(1.05);
    }

    .media-caption {
      position: absolute;
      bottom: 0;
      left: 0;
      right: 0;

      padding: 25px;

      background: linear-gradient(
        transparent,
        rgba(0, 0, 0, 0.95)
      );
    }

    .media-caption h3 {
      color: #fff;
    }

    .media-caption p {
      color: #aaa;
      font-size: 14px;
    }

    /* =========================
       BOOKING / CONTACT
    ========================= */

    .contact {
      text-align: center;
    }

    .contact-box {
      background:
        radial-gradient(
          circle at center,
          rgba(212, 175, 55, 0.13),
          transparent 60%
        ),
        #0b0b0b;

      border: 1px solid rgba(212, 175, 55, 0.3);
      padding: 70px 30px;
    }

    .contact-box h2 {
      font-size: clamp(40px, 7vw, 75px);
      line-height: 1;
      margin-bottom: 20px;
    }

    .contact-box p {
      color: var(--gray);
      max-width: 600px;
      margin: 0 auto 30px;
    }

    .contact-details {
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
      gap: 25px;
      margin-top: 30px;
    }

    .contact-details a {
      color: var(--gold);
      font-weight: bold;
    }

    /* =========================
       FOOTER
    ========================= */

    footer {
      border-top: 1px solid #222;
      padding: 30px 5%;
      background: #030303;

      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 20px;
    }

    footer p {
      color: #777;
      font-size: 13px;
    }

    .footer-logo {
      color: var(--gold);
      font-weight: bold;
      letter-spacing: 2px;
    }

    /* =========================
       ANIMATIONS
    ========================= */

    @keyframes rotate {
      from {
        transform: rotate(0deg);
      }

      to {
        transform: rotate(360deg);
      }
    }

    @keyframes glow {
      0%, 100% {
        opacity: 0.5;
        transform: scale(0.95);
      }

      50% {
        opacity: 1;
        transform: scale(1.05);
      }
    }

    /* =========================
       RESPONSIVE
    ========================= */

    @media (max-width: 900px) {

      .nav {
        min-height: 70px;
      }

      nav {
        gap: 15px;
      }

      nav a {
        font-size: 12px;
      }

      .hero {
        grid-template-columns: 1fr;
        text-align: center;
        gap: 40px;
      }

      .hero-description {
        margin-left: auto;
        margin-right: auto;
      }

      .buttons {
        justify-content: center;
      }

      .hero-image {
        min-height: 500px;
      }

      .hero-image img {
        height: 500px;
      }

      .about-inner {
        grid-template-columns: 1fr;
      }

      .about-image img {
        margin: auto;
      }

      .services-grid {
        grid-template-columns: repeat(2, 1fr);
      }
    }

    @media (max-width: 600px) {

      .nav {
        width: 94%;
      }

      .logo {
        font-size: 18px;
      }

      nav {
        gap: 10px;
      }

      nav a {
        font-size: 11px;
      }

      .nav-book {
        padding: 8px 11px;
      }

      section {
        padding: 75px 0;
      }

      .hero {
        width: 90%;
        padding-top: 55px;
      }

      .hero h1 {
        font-size: 58px;
        letter-spacing: -3px;
      }

      .hero-description {
        font-size: 15px;
      }

      .hero-image {
        min-height: 420px;
      }

      .hero-image::before {
        width: 300px;
        height: 300px;
      }

      .hero-image::after {
        width: 350px;
        height: 350px;
      }

      .hero-image img {
        width: 85%;
        height: 420px;
      }

      .facts {
        grid-template-columns: 1fr;
      }

      .services-grid {
        grid-template-columns: 1fr;
      }

      .media-grid {
        grid-template-columns: 1fr;
      }

      .media-card img {
        height: 430px;
      }

      footer {
        flex-direction: column;
        text-align: center;
      }
    }

    @media (max-width: 420px) {

      nav a:not(.nav-book) {
        display: none;
      }

      .hero h1 {
        font-size: 50px;
      }

      .hero-image img {
        width: 90%;
      }

      .buttons {
        flex-direction: column;
      }

      .btn {
        width: 100%;
      }
    }

    @media (prefers-reduced-motion: reduce) {
      *,
      *::before,
      *::after {
        scroll-behavior: auto !important;
        animation: none !important;
        transition: none !important;
      }
    }
  </style>
</head>

<body>

  <!-- =========================
       HEADER
  ========================== -->

  <header>
    <div class="nav">

      <a href="index.html" class="logo">
        BIG <span>SHIZZY</span>
      </a>

      <nav>
        <a href="about.html">About</a>
        <a href="#services">Services</a>
        <a href="#media">Media</a>
        <a href="#contact" class="nav-book">Book Him</a>
      </nav>

    </div>
  </header>


  <!-- =========================
       HERO
  ========================== -->

  <main>

    <section class="hero">

      <div class="hero-content">

        <span class="eyebrow">
          Artist • Entertainer • Creative
        </span>

        <h1>
          BIG<br>
          <span>SHIZZY</span>
        </h1>

        <p class="hero-description">
          Welcome to the official website of Big Shizzy —
          an artist and entertainer from Ogun State, Nigeria,
          building a creative identity through music,
          entertainment, branding and media.
        </p>

        <div class="buttons">

          <a
            href="https://wa.me/2349070804147"
            target="_blank"
            class="btn btn-gold"
          >
            Book Big Shizzy
          </a>

          <a
            href="about.html"
            class="btn btn-outline"
          >
            Explore His Story
          </a>

        </div>

      </div>


      <div class="hero-image">

        <!--
          IMPORTANT:
          Make sure this exact image is uploaded
          to the same folder as this index.html file.
        -->

        <img
          src="E94E2B62-8DA5-4B74-B19C-E97D8F87F49C.jpeg"
          alt="Big Shizzy"
        >

      </div>

    </section>


    <!-- =========================
         ABOUT PREVIEW
    ========================== -->

    <section class="about" id="about">

      <div class="about-inner">

        <div class="about-image">

          <img
            src="E94E2B62-8DA5-4B74-B19C-E97D8F87F49C.jpeg"
            alt="Big Shizzy portrait"
          >

        </div>


        <div class="about-content">

          <small>Get To Know Him</small>

          <h2>
            About<br>
            Big Shizzy
          </h2>

          <p>
            Big Shizzy, also known as Toluwani, is an artist
            and entertainer from Ogun State, Nigeria.
          </p>

          <p>
            His creative interests span music, entertainment,
            barbing and painting, giving him different ways
            to express his creativity.
          </p>

          <p>
            He is also developing a professional platform
            focused on artist promotion, branding,
            entertainment and media services.
          </p>


          <div class="facts">

            <div class="fact">
              <strong>Full Name</strong>
              <span>Toluwani</span>
            </div>

            <div class="fact">
              <strong>Date of Birth</strong>
              <span>March 22</span>
            </div>

            <div class="fact">
              <strong>State of Origin</strong>
              <span>Ogun State, Nigeria</span>
            </div>

            <div class="fact">
              <strong>Creative Focus</strong>
              <span>Music & Entertainment</span>
            </div>

          </div>


          <!-- THIS OPENS THE NEW ABOUT PAGE -->

          <a href="about.html" class="about-link">
            Get To Know Big Shizzy →
          </a>

        </div>

      </div>

    </section>


    <!-- =========================
         SERVICES
    ========================== -->

    <section id="services">

      <div class="section-heading">

        <small>What He Does</small>

        <h2>
          Creative<br>
          Services
        </h2>

        <p>
          Big Shizzy's creative platform covers
          entertainment, artist development, branding
          and media-related services.
        </p>

      </div>


      <div class="services-grid">

        <div class="service-card">
          <span class="service-number">01</span>
          <h3>Artist Promotion</h3>
        </div>

        <div class="service-card">
          <span class="service-number">02</span>
          <h3>Artist Branding</h3>
        </div>

        <div class="service-card">
          <span class="service-number">03</span>
          <h3>Event Hosting</h3>
        </div>

        <div class="service-card">
          <span class="service-number">04</span>
          <h3>Brand Influencing</h3>
        </div>

        <div class="service-card">
          <span class="service-number">05</span>
          <h3>Talent Management</h3>
        </div>

        <div class="service-card">
          <span class="service-number">06</span>
          <h3>Music & Video Production</h3>
        </div>

        <div class="service-card">
          <span class="service-number">07</span>
          <h3>Music Distribution</h3>
        </div>

        <div class="service-card">
          <span class="service-number">08</span>
          <h3>Modeling</h3>
        </div>

        <div class="service-card">
          <span class="service-number">09</span>
          <h3>Radio & TV</h3>
        </div>

      </div>

    </section>


    <!-- =========================
         MEDIA
    ========================== -->

    <section class="media" id="media">

      <div class="media-inner">

        <div class="section-heading">

          <small>Visuals</small>

          <h2>
            Big Shizzy<br>
            Media
          </h2>

          <p>
            A selection of Big Shizzy's artist and
            promotional visuals.
          </p>

        </div>


        <div class="media-grid">

          <div class="media-card">

            <img
              src="E94E2B62-8DA5-4B74-B19C-E97D8F87F49C.jpeg"
              alt="Big Shizzy artist portrait"
            >

            <div class="media-caption">

              <h3>Artist Profile</h3>

              <p>
                Big Shizzy — Artist & Entertainer
              </p>

            </div>

          </div>


          <div class="media-card">

            <img
              src="01159400-FA46-4488-980C-670B53929D2A.jpeg"
              alt="Big Shizzy promotional flyer"
            >

            <div class="media-caption">

              <h3>Promotional Visual</h3>

              <p>
                Big Shizzy entertainment and media
              </p>

            </div>

          </div>

        </div>

      </div>

    </section>


    <!-- =========================
         CONTACT
    ========================== -->

    <section class="contact" id="contact">

      <div class="contact-box">

        <div class="section-heading">

          <small>Bookings & Enquiries</small>

          <h2>
            Let's Work<br>
            Together.
          </h2>

          <p>
            For bookings, collaborations, entertainment
            services and business enquiries, contact
            Big Shizzy directly.
          </p>

        </div>


        <div class="buttons">

          <a
            href="https://wa.me/2349070804147"
            target="_blank"
            class="btn btn-gold"
          >
            WhatsApp Big Shizzy
          </a>

          <a
            href="mailto:adeshipe94@gmail.com"
            class="btn btn-outline"
          >
            Send Email
          </a>

        </div>


        <div class="contact-details">

          <a href="https://wa.me/2349070804147" target="_blank">
            +234 907 080 4147
          </a>

          <a href="mailto:adeshipe94@gmail.com">
            adeshipe94@gmail.com
          </a>

        </div>

      </div>

    </section>

  </main>


  <!-- =========================
       FOOTER
  ========================== -->

  <footer>

    <div class="footer-logo">
      BIG SHIZZY
    </div>

    <p>
      © <span id="year"></span> Big Shizzy.
      All Rights Reserved.
    </p>

    <p>
      Artist • Entertainer • Creative
    </p>

  </footer>


  <script>
    document.getElementById("year").textContent =
      new Date().getFullYear();
  </script>

</body>
</html>
