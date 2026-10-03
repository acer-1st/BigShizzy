<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Big Shizzy | Artist • Entertainer • Creative</title>

    <meta name="description"
          content="Official website of Big Shizzy (Toluwani) — artist, entertainer, barber, painter and creative professional from Ogun State, Nigeria.">

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            scroll-behavior: smooth;
        }

        :root {
            --black: #050505;
            --dark: #0c0c0c;
            --gold: #d4af37;
            --light-gold: #f4d675;
            --white: #ffffff;
            --gray: #aaaaaa;
            --card: #111111;
        }

        body {
            font-family: Arial, Helvetica, sans-serif;
            background: var(--black);
            color: var(--white);
            line-height: 1.6;
        }

        /* ================= HEADER ================= */

        header {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            z-index: 1000;
            background: rgba(0, 0, 0, 0.92);
            backdrop-filter: blur(12px);
            border-bottom: 1px solid rgba(212, 175, 55, 0.2);
        }

        .nav {
            max-width: 1200px;
            margin: auto;
            padding: 18px 25px;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 25px;
            font-weight: 900;
            letter-spacing: 2px;
            color: var(--gold);
        }

        .logo span {
            color: white;
        }

        nav ul {
            display: flex;
            list-style: none;
            gap: 28px;
        }

        nav a {
            color: white;
            text-decoration: none;
            font-size: 14px;
            font-weight: bold;
            transition: 0.3s;
        }

        nav a:hover {
            color: var(--gold);
        }

        /* ================= HERO ================= */

        .hero {
            min-height: 100vh;
            padding: 120px 25px 70px;
            display: flex;
            align-items: center;
            position: relative;
            overflow: hidden;
            background:
                radial-gradient(circle at 75% 40%, rgba(212,175,55,0.15), transparent 35%),
                linear-gradient(135deg, #050505, #111111);
        }

        .hero-container {
            max-width: 1200px;
            width: 100%;
            margin: auto;
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 60px;
            align-items: center;
        }

        .hero-text h1 {
            font-size: clamp(55px, 8vw, 105px);
            line-height: 0.95;
            font-weight: 900;
            letter-spacing: -3px;
        }

        .hero-text h1 span {
            color: var(--gold);
        }

        .hero-subtitle {
            margin-top: 25px;
            color: var(--light-gold);
            font-size: 20px;
            letter-spacing: 3px;
            text-transform: uppercase;
        }

        .hero-text p {
            margin-top: 20px;
            max-width: 550px;
            color: var(--gray);
            font-size: 17px;
        }

        .buttons {
            display: flex;
            gap: 15px;
            margin-top: 35px;
            flex-wrap: wrap;
        }

        .btn {
            display: inline-block;
            padding: 14px 25px;
            border-radius: 4px;
            text-decoration: none;
            font-weight: bold;
            transition: 0.3s;
        }

        .btn-gold {
            background: var(--gold);
            color: #000;
        }

        .btn-gold:hover {
            background: var(--light-gold);
            transform: translateY(-3px);
        }

        .btn-outline {
            border: 1px solid var(--gold);
            color: var(--gold);
        }

        .btn-outline:hover {
            background: var(--gold);
            color: black;
        }

        /* HERO IMAGE */

        .hero-image {
            display: flex;
            justify-content: center;
            position: relative;
        }

        .hero-image img {
            width: min(440px, 90%);
            max-height: 650px;
            object-fit: cover;
            border-radius: 8px;
            border: 2px solid rgba(212,175,55,0.5);
            box-shadow: 0 0 70px rgba(212,175,55,0.18);
        }

        /* ================= GENERAL ================= */

        section {
            padding: 100px 25px;
        }

        .container {
            max-width: 1100px;
            margin: auto;
        }

        .section-title {
            text-align: center;
            margin-bottom: 55px;
        }

        .section-title small {
            color: var(--gold);
            text-transform: uppercase;
            letter-spacing: 3px;
            font-weight: bold;
        }

        .section-title h2 {
            margin-top: 10px;
            font-size: clamp(35px, 5vw, 55px);
        }

        .section-title p {
            color: var(--gray);
            max-width: 650px;
            margin: 15px auto 0;
        }

        /* ================= ABOUT ================= */

        .about {
            background: #090909;
        }

        .about-grid {
            display: grid;
            grid-template-columns: 0.8fr 1.2fr;
            gap: 60px;
            align-items: center;
        }

        .about-image img {
            width: 100%;
            border-radius: 8px;
            border: 1px solid rgba(212,175,55,0.4);
        }

        .about-content h3 {
            color: var(--gold);
            font-size: 30px;
            margin-bottom: 15px;
        }

        .about-content p {
            color: #c5c5c5;
            margin-bottom: 18px;
        }

        .facts {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 15px;
            margin-top: 30px;
        }

        .fact {
            background: var(--card);
            border: 1px solid #222;
            padding: 18px;
            border-radius: 6px;
        }

        .fact strong {
            color: var(--gold);
            display: block;
            margin-bottom: 5px;
        }

        /* ================= SERVICES ================= */

        .services {
            background: var(--black);
        }

        .services-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 20px;
        }

        .service-card {
            background: var(--card);
            padding: 30px 25px;
            border: 1px solid #222;
            border-radius: 8px;
            transition: 0.3s;
        }

        .service-card:hover {
            transform: translateY(-8px);
            border-color: var(--gold);
            box-shadow: 0 10px 30px rgba(212,175,55,0.08);
        }

        .service-number {
            font-size: 14px;
            color: var(--gold);
            font-weight: bold;
        }

        .service-card h3 {
            margin: 15px 0 10px;
            font-size: 21px;
        }

        .service-card p {
            color: var(--gray);
            font-size: 14px;
        }

        /* ================= MEDIA ================= */

        .media {
            background: #090909;
        }

        .media-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 25px;
        }

        .media-card {
            overflow: hidden;
            border-radius: 8px;
            border: 1px solid #252525;
            background: #111;
        }

        .media-card img {
            width: 100%;
            display: block;
            transition: 0.5s;
        }

        .media-card:hover img {
            transform: scale(1.04);
        }

        .media-caption {
            padding: 20px;
        }

        .media-caption h3 {
            color: var(--gold);
            margin-bottom: 5px;
        }

        .media-caption p {
            color: var(--gray);
        }

        /* ================= CONTACT ================= */

        .contact {
            text-align: center;
            background:
                radial-gradient(circle at center, rgba(212,175,55,0.1), transparent 50%),
                #050505;
        }

        .contact-box {
            max-width: 800px;
            margin: auto;
            padding: 50px 25px;
            border: 1px solid rgba(212,175,55,0.3);
            border-radius: 10px;
            background: rgba(255,255,255,0.02);
        }

        .contact-box h2 {
            font-size: clamp(35px, 6vw, 55px);
            margin-bottom: 15px;
        }

        .contact-box > p {
            color: var(--gray);
            margin-bottom: 35px;
        }

        .contact-details {
            display: flex;
            justify-content: center;
            gap: 20px;
            flex-wrap: wrap;
            margin-bottom: 30px;
        }

        .contact-item {
            background: #111;
            padding: 18px 25px;
            border-radius: 6px;
            border: 1px solid #222;
        }

        .contact-item strong {
            color: var(--gold);
            display: block;
            margin-bottom: 5px;
        }

        .contact-item a {
            color: white;
            text-decoration: none;
        }

        .contact-item a:hover {
            color: var(--gold);
        }

        /* ================= FOOTER ================= */

        footer {
            background: #000;
            border-top: 1px solid #1c1c1c;
            padding: 30px 20px;
            text-align: center;
        }

        footer .footer-logo {
            color: var(--gold);
            font-size: 22px;
            font-weight: bold;
            letter-spacing: 2px;
        }

        footer p {
            color: #777;
            margin-top: 8px;
            font-size: 13px;
        }

        /* ================= MOBILE ================= */

        @media (max-width: 850px) {

            nav ul {
                gap: 14px;
            }

            nav a {
                font-size: 12px;
            }

            .hero-container {
                grid-template-columns: 1fr;
                text-align: center;
            }

            .hero-text p {
                margin-left: auto;
                margin-right: auto;
            }

            .buttons {
                justify-content: center;
            }

            .hero-image {
                order: -1;
            }

            .hero-image img {
                width: min(350px, 85%);
            }

            .about-grid {
                grid-template-columns: 1fr;
            }

            .about-image {
                max-width: 500px;
                margin: auto;
            }

            .services-grid {
                grid-template-columns: 1fr 1fr;
            }
        }

        @media (max-width: 600px) {

            .nav {
                padding: 15px;
            }

            .logo {
                font-size: 19px;
            }

            nav ul {
                gap: 10px;
            }

            nav a {
                font-size: 10px;
            }

            section {
                padding: 75px 18px;
            }

            .hero {
                padding-top: 110px;
            }

            .hero-text h1 {
                font-size: 60px;
            }

            .hero-subtitle {
                font-size: 14px;
                letter-spacing: 2px;
            }

            .hero-text p {
                font-size: 15px;
            }

            .services-grid {
                grid-template-columns: 1fr;
            }

            .media-grid {
                grid-template-columns: 1fr;
            }

            .facts {
                grid-template-columns: 1fr;
            }

            .contact-details {
                flex-direction: column;
            }
        }
    </style>
</head>

<body>

<!-- ================= HEADER ================= -->

<header>
    <div class="nav">

        <div class="logo">
            BIG <span>SHIZZY</span>
        </div>

        <nav>
            <ul>
                <li><a href="#about">About</a></li>
                <li><a href="#services">Services</a></li>
                <li><a href="#media">Media</a></li>
                <li><a href="#contact">Book</a></li>
            </ul>
        </nav>

    </div>
</header>


<!-- ================= HERO ================= -->

<section class="hero">

    <div class="hero-container">

        <div class="hero-text">

            <div class="hero-subtitle">
                Artist • Entertainer • Creative
            </div>

            <h1>
                BIG<br>
                <span>SHIZZY</span>
            </h1>

            <p>
                Meet Big Shizzy — also known as Toluwani.
                An artist, entertainer and creative professional
                bringing music, style and creativity together.
            </p>

            <div class="buttons">

                <a class="btn btn-gold"
                   href="https://wa.me/2349070804147"
                   target="_blank">
                    Book Big Shizzy
                </a>

                <a class="btn btn-outline"
                   href="#services">
                    View Services
                </a>

            </div>

        </div>


        <div class="hero-image">

            <img src="E94E2B62-8DA5-4B74-B19C-E97D8F87F49C.jpeg"
                 alt="Big Shizzy">

        </div>

    </div>

</section>


<!-- ================= ABOUT ================= -->

<section class="about" id="about">

    <div class="container">

        <div class="section-title">

            <small>Get To Know Him</small>

            <h2>About Big Shizzy</h2>

            <p>
                Creativity, entertainment and passion in one personality.
            </p>

        </div>


        <div class="about-grid">

            <div class="about-image">

                <img src="E94E2B62-8DA5-4B74-B19C-E97D8F87F49C.jpeg"
                     alt="Big Shizzy portrait">

            </div>


            <div class="about-content">

                <h3>Big Shizzy (Toluwani)</h3>

                <p>
                    Big Shizzy is an artist and entertainer from
                    Ogun State, Nigeria, with a passion for creativity
                    and entertainment.
                </p>

                <p>
                    His interests and professional activities cover
                    music, barbing and painting, allowing him to
                    express creativity across different areas.
                </p>

                <p>
                    Through artist promotion, branding, entertainment
                    and media services, Big Shizzy is building a
                    professional platform for artists, brands and
                    entertainment projects.
                </p>


                <div class="facts">

                    <div class="fact">
                        <strong>Full Name</strong>
                        Toluwani
                    </div>

                    <div class="fact">
                        <strong>Date of Birth</strong>
                        March 22
                    </div>

                    <div class="fact">
                        <strong>State of Origin</strong>
                        Ogun State, Nigeria
                    </div>

                    <div class="fact">
                        <strong>Hobby</strong>
                        Entertainment
                    </div>

                </div>

            </div>

        </div>

    </div>

</section>


<!-- ================= SERVICES ================= -->

<section class="services" id="services">

    <div class="container">

        <div class="section-title">

            <small>What We Do</small>

            <h2>Our Services</h2>

            <p>
                Professional entertainment, creative and media services.
            </p>

        </div>


        <div class="services-grid">


            <div class="service-card">

                <div class="service-number">01</div>

                <h3>Artist Promotion</h3>

                <p>
                    Helping artists gain visibility and connect
                    with a wider audience.
                </p>

            </div>


            <div class="service-card">

                <div class="service-number">02</div>

                <h3>Artist Branding</h3>

                <p>
                    Building strong and professional identities
                    for artists and entertainers.
                </p>

            </div>


            <div class="service-card">

                <div class="service-number">03</div>

                <h3>Event Hosting</h3>

                <p>
                    Entertainment and hosting services for events,
                    shows and special occasions.
                </p>

            </div>


            <div class="service-card">

                <div class="service-number">04</div>

                <h3>Brand Influencing</h3>

                <p>
                    Connecting brands with entertainment and
                    creative audiences.
                </p>

            </div>


            <div class="service-card">

                <div class="service-number">05</div>

                <h3>Talent Management</h3>

                <p>
                    Supporting creative talents with promotion,
                    branding and career development.
                </p>

            </div>


            <div class="service-card">

                <div class="service-number">06</div>

                <h3>Music & Video Production</h3>

                <p>
                    Creative support for music and video projects
                    from concept to production.
                </p>

            </div>


            <div class="service-card">

                <div class="service-number">07</div>

                <h3>Music Distribution</h3>

                <p>
                    Helping artists get their music ready for
                    distribution and wider exposure.
                </p>

            </div>


            <div class="service-card">

                <div class="service-number">08</div>

                <h3>Modeling</h3>

                <p>
                    Creative modeling and promotional opportunities
                    for brands and entertainment projects.
                </p>

            </div>


            <div class="service-card">

                <div class="service-number">09</div>

                <h3>Radio & TV</h3>

                <p>
                    Radio airplay, radio tours, TV airplay and
                    TV interview opportunities.
                </p>

            </div>


        </div>

    </div>

</section>


<!-- ================= MEDIA ================= -->

<section class="media" id="media">

    <div class="container">

        <div class="section-title">

            <small>Portfolio</small>

            <h2>Media & Work</h2>

            <p>
                A glimpse into the Big Shizzy brand.
            </p>

        </div>


        <div class="media-grid">


            <div class="media-card">

                <img src="01159400-FA46-4488-980C-670B53929D2A.jpeg"
                     alt="Big Shizzy services flyer">

                <div class="media-caption">

                    <h3>Entertainment & Promotion</h3>

                    <p>
                        Artist promotion, branding, media exposure
                        and entertainment services.
                    </p>

                </div>

            </div>


            <div class="media-card">

                <img src="E94E2B62-8DA5-4B74-B19C-E97D8F87F49C.jpeg"
                     alt="Big Shizzy">

                <div class="media-caption">

                    <h3>Big Shizzy</h3>

                    <p>
                        Artist • Entertainer • Creative
                    </p>

                </div>

            </div>


        </div>

    </div>

</section>


<!-- ================= CONTACT ================= -->

<section class="contact" id="contact">

    <div class="container">

        <div class="contact-box">

            <h2>Let's Work Together</h2>

            <p>
                For bookings, collaborations, artist promotion,
                branding, events and other enquiries, get in touch.
            </p>


            <div class="contact-details">

                <div class="contact-item">

                    <strong>WhatsApp</strong>

                    <a href="https://wa.me/2349070804147"
                       target="_blank">
                        +234 907 080 4147
                    </a>

                </div>


                <div class="contact-item">

                    <strong>Email</strong>

                    <a href="mailto:adeshipe94@gmail.com">
                        adeshipe94@gmail.com
                    </a>

                </div>

            </div>


            <a class="btn btn-gold"
               href="https://wa.me/2349070804147?text=Hello%20Big%20Shizzy,%20I%20would%20like%20to%20make%20an%20enquiry."
               target="_blank">

                Contact Big Shizzy

            </a>

        </div>

    </div>

</section>


<!-- ================= FOOTER ================= -->

<footer>

    <div class="footer-logo">
        BIG SHIZZY
    </div>

    <p>
        © <span id="year"></span> Big Shizzy. All Rights Reserved.
    </p>

    <p>
        Artist • Entertainer • Creative
    </p>

</footer>


<!-- ================= JAVASCRIPT ================= -->

<script>

    // Automatically update copyright year
    document.getElementById("year").textContent =
        new Date().getFullYear();

</script>

</body>
</html>
