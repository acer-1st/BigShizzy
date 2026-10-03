<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">

<meta name="viewport"
      content="width=device-width, initial-scale=1.0, maximum-scale=1.0">

<title>Big Shizzy | Artist • Entertainer • Creative</title>

<meta name="description"
content="Official website of Big Shizzy (Toluwani) — artist, entertainer, barber, painter and creative professional from Ogun State, Nigeria.">

<style>

/* =====================================================
   RESET
===================================================== */

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
}

body {
    width: 100%;
    min-width: 0;
    overflow-x: hidden;

    font-family: Arial, Helvetica, sans-serif;

    background: #050505;
    color: #ffffff;

    line-height: 1.6;
}

img {
    max-width: 100%;
}

a {
    -webkit-tap-highlight-color: transparent;
}


/* =====================================================
   COLORS
===================================================== */

:root {
    --black: #050505;
    --dark: #0b0b0b;
    --card: #111111;

    --gold: #d4af37;
    --light-gold: #f3d76b;

    --white: #ffffff;
    --gray: #aaaaaa;
    --border: #242424;
}


/* =====================================================
   HEADER
===================================================== */

header {
    position: fixed;
    top: 0;
    left: 0;

    width: 100%;
    height: 72px;

    z-index: 9999;

    background: rgba(0,0,0,0.94);

    backdrop-filter: blur(15px);
    -webkit-backdrop-filter: blur(15px);

    border-bottom: 1px solid rgba(212,175,55,0.22);
}

.nav {
    width: 100%;
    max-width: 1200px;

    height: 100%;

    margin: 0 auto;
    padding: 0 25px;

    display: flex;
    justify-content: space-between;
    align-items: center;
}

.logo {
    font-size: 22px;
    font-weight: 900;

    letter-spacing: 2px;

    color: var(--gold);

    white-space: nowrap;
}

.logo span {
    color: white;
}

nav ul {
    display: flex;
    align-items: center;

    list-style: none;

    gap: 25px;
}

nav a {
    color: white;
    text-decoration: none;

    font-size: 13px;
    font-weight: bold;

    transition: 0.3s;
}

nav a:hover {
    color: var(--gold);
}


/* =====================================================
   HERO
===================================================== */

.hero {
    width: 100%;
    min-height: 100vh;

    padding: 120px 25px 80px;

    display: flex;
    align-items: center;

    background:
        radial-gradient(
            circle at 75% 40%,
            rgba(212,175,55,0.15),
            transparent 35%
        ),
        linear-gradient(
            135deg,
            #050505,
            #111111
        );
}

.hero-container {
    width: 100%;
    max-width: 1150px;

    margin: 0 auto;

    display: grid;

    grid-template-columns:
        minmax(0, 1fr)
        minmax(0, 1fr);

    gap: 60px;

    align-items: center;
}

.hero-text {
    min-width: 0;
}

.hero-subtitle {
    margin-bottom: 20px;

    color: var(--light-gold);

    font-size: 15px;

    letter-spacing: 3px;

    text-transform: uppercase;

    font-weight: bold;
}

.hero-text h1 {
    font-size: clamp(55px, 8vw, 105px);

    line-height: 0.9;

    font-weight: 900;

    letter-spacing: -4px;
}

.hero-text h1 span {
    color: var(--gold);
}

.hero-text p {
    max-width: 560px;

    margin-top: 25px;

    color: var(--gray);

    font-size: 17px;
}

.buttons {
    display: flex;

    flex-wrap: wrap;

    gap: 14px;

    margin-top: 32px;
}

.btn {
    display: inline-flex;

    align-items: center;
    justify-content: center;

    min-height: 50px;

    padding: 13px 25px;

    border-radius: 5px;

    text-decoration: none;

    font-weight: bold;

    transition: 0.3s;

    cursor: pointer;
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

    background: transparent;
}

.btn-outline:hover {
    background: var(--gold);

    color: #000;
}


/* =====================================================
   HERO IMAGE
===================================================== */

.hero-image {
    width: 100%;

    display: flex;

    justify-content: center;

    align-items: center;
}

.hero-photo {
    width: min(430px, 100%);

    aspect-ratio: 4 / 5;

    object-fit: cover;

    display: block;

    border-radius: 10px;

    border: 2px solid rgba(212,175,55,0.55);

    box-shadow:
        0 0 70px rgba(212,175,55,0.18);
}


/* Image fallback */

.image-fallback {
    width: min(430px, 100%);

    aspect-ratio: 4 / 5;

    border-radius: 10px;

    border: 2px solid rgba(212,175,55,0.55);

    background:
        radial-gradient(
            circle at center,
            rgba(212,175,55,0.18),
            transparent 60%
        ),
        #101010;

    display: none;

    align-items: center;
    justify-content: center;

    text-align: center;

    box-shadow:
        0 0 70px rgba(212,175,55,0.12);
}

.image-fallback div {
    padding: 20px;
}

.image-fallback strong {
    display: block;

    font-size: 42px;

    line-height: 1;

    color: white;
}

.image-fallback span {
    display: block;

    margin-top: 10px;

    color: var(--gold);

    font-weight: bold;

    letter-spacing: 3px;
}


/* =====================================================
   GENERAL SECTIONS
===================================================== */

section {
    width: 100%;

    padding: 100px 25px;
}

.container {
    width: 100%;
    max-width: 1100px;

    margin: 0 auto;
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

    font-size: clamp(34px, 5vw, 55px);

    line-height: 1.1;
}

.section-title p {
    max-width: 650px;

    margin: 15px auto 0;

    color: var(--gray);
}


/* =====================================================
   ABOUT
===================================================== */

.about {
    background: #090909;
}

.about-grid {
    width: 100%;

    display: grid;

    grid-template-columns:
        minmax(0, 0.8fr)
        minmax(0, 1.2fr);

    gap: 55px;

    align-items: center;
}

.about-image {
    width: 100%;
}

.about-image img {
    width: 100%;

    aspect-ratio: 4 / 5;

    object-fit: cover;

    display: block;

    border-radius: 10px;

    border: 1px solid rgba(212,175,55,0.4);
}

.about-content {
    min-width: 0;
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
    width: 100%;

    display: grid;

    grid-template-columns: repeat(2, minmax(0,1fr));

    gap: 15px;

    margin-top: 30px;
}

.fact {
    background: var(--card);

    border: 1px solid var(--border);

    padding: 18px;

    border-radius: 7px;
}

.fact strong {
    color: var(--gold);

    display: block;

    margin-bottom: 5px;
}


/* =====================================================
   SERVICES
===================================================== */

.services {
    background: #050505;
}

.services-grid {
    display: grid;

    grid-template-columns:
        repeat(3, minmax(0,1fr));

    gap: 20px;
}

.service-card {
    background: var(--card);

    padding: 30px 25px;

    border: 1px solid var(--border);

    border-radius: 8px;

    transition: 0.3s;
}

.service-card:hover {
    transform: translateY(-7px);

    border-color: var(--gold);

    box-shadow:
        0 10px 30px rgba(212,175,55,0.08);
}

.service-number {
    color: var(--gold);

    font-size: 14px;

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


/* =====================================================
   MEDIA
===================================================== */

.media {
    background: #090909;
}

.media-grid {
    display: grid;

    grid-template-columns:
        repeat(2, minmax(0,1fr));

    gap: 25px;
}

.media-card {
    overflow: hidden;

    border-radius: 8px;

    border: 1px solid var(--border);

    background: #111;
}

.media-card img {
    width: 100%;

    aspect-ratio: 16 / 10;

    object-fit: cover;

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


/* =====================================================
   CONTACT
===================================================== */

.contact {
    text-align: center;

    background:
        radial-gradient(
            circle at center,
            rgba(212,175,55,0.1),
            transparent 50%
        ),
        #050505;
}

.contact-box {
    width: 100%;
    max-width: 800px;

    margin: auto;

    padding: 50px 25px;

    border: 1px solid rgba(212,175,55,0.3);

    border-radius: 10px;

    background: rgba(255,255,255,0.02);
}

.contact-box h2 {
    font-size: clamp(34px, 6vw, 55px);

    line-height: 1.1;

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

    border: 1px solid var(--border);
}

.contact-item strong {
    color: var(--gold);

    display: block;

    margin-bottom: 5px;
}

.contact-item a {
    color: white;

    text-decoration: none;

    word-break: break-word;
}

.contact-item a:hover {
    color: var(--gold);
}


/* =====================================================
   FOOTER
===================================================== */

footer {
    width: 100%;

    background: #000;

    border-top: 1px solid #1c1c1c;

    padding: 30px 20px;

    text-align: center;
}

.footer-logo {
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


/* =====================================================
   TABLET
===================================================== */

@media (max-width: 850px) {

    .hero-container {
        grid-template-columns: 1fr;

        gap: 45px;

        text-align: center;
    }

    .hero-image {
        order: -1;
    }

    .hero-photo,
    .image-fallback {
        width: min(360px, 85vw);
    }

    .hero-text p {
        margin-left: auto;
        margin-right: auto;
    }

    .buttons {
        justify-content: center;
    }

    .about-grid {
        grid-template-columns: 1fr;

        gap: 40px;
    }

    .about-image {
        max-width: 500px;

        margin: 0 auto;
    }

    .services-grid {
        grid-template-columns:
            repeat(2, minmax(0,1fr));
    }
}


/* =====================================================
   MOBILE
===================================================== */

@media (max-width: 600px) {

    header {
        height: 64px;
    }

    .nav {
        padding: 0 15px;
    }

    .logo {
        font-size: 17px;

        letter-spacing: 1.5px;
    }

    nav ul {
        gap: 9px;
    }

    nav a {
        font-size: 9px;
    }

    section {
        padding: 75px 16px;
    }

    .hero {
        min-height: auto;

        padding:
            105px
            16px
            75px;
    }

    .hero-container {
        width: 100%;

        grid-template-columns: 1fr;

        gap: 35px;
    }

    .hero-subtitle {
        font-size: 11px;

        letter-spacing: 2px;
    }

    .hero-text h1 {
        font-size: clamp(55px, 17vw, 78px);

        letter-spacing: -3px;
    }

    .hero-text p {
        font-size: 15px;

        line-height: 1.7;
    }

    .hero-photo,
    .image-fallback {
        width: min(310px, 88vw);
    }

    .buttons {
        width: 100%;

        flex-direction: column;

        align-items: stretch;
    }

    .btn {
        width: 100%;
    }

    .section-title {
        margin-bottom: 40px;
    }

    .section-title small {
        font-size: 11px;

        letter-spacing: 2px;
    }

    .section-title h2 {
        font-size: 34px;
    }

    .section-title p {
        font-size: 14px;
    }

    .about-content h3 {
        font-size: 25px;
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

    .contact-box {
        padding: 40px 18px;
    }

    .contact-details {
        flex-direction: column;
    }

    .contact-item {
        width: 100%;
    }
}


/* =====================================================
   VERY SMALL PHONES
===================================================== */

@media (max-width: 380px) {

    nav ul {
        gap: 6px;
    }

    nav a {
        font-size: 8px;
    }

    .logo {
        font-size: 15px;
    }

    .hero-text h1 {
        font-size: 55px;
    }
}

</style>
</head>


<body>


<!-- =====================================================
     HEADER
===================================================== -->

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


<!-- =====================================================
     HERO
===================================================== -->

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

                <a
                    class="btn btn-gold"
                    href="https://wa.me/2349070804147"
                    target="_blank"
                    rel="noopener">
                    Book Big Shizzy
                </a>

                <a
                    class="btn btn-outline"
                    href="#services">
                    View Services
                </a>

            </div>

        </div>


        <div class="hero-image">

            <img
                class="hero-photo"
                src="E94E2B62-8DA5-4B74-B19C-E97D8F87F49C.jpeg"
                alt="Big Shizzy">

            <div class="image-fallback">
                <div>
                    <strong>BIG</strong>
                    <strong>SHIZZY</strong>
                    <span>ARTIST • CREATIVE</span>
                </div>
            </div>

        </div>


    </div>

</section>


<!-- =====================================================
     ABOUT
===================================================== -->

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

                <img
                    src="E94E2B62-8DA5-4B74-B19C-E97D8F87F49C.jpeg"
                    alt="Big Shizzy portrait">

            </div>


            <div class="about-content">

                <h3>
                    Big Shizzy (Toluwani)
                </h3>

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


<!-- =====================================================
     SERVICES
===================================================== -->

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


<!-- =====================================================
     MEDIA
===================================================== -->

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

                <img
                    src="01159400-FA46-4488-980C-670B53929D2A.jpeg"
                    alt="Big Shizzy services flyer">

                <div class="media-caption">

                    <h3>
                        Entertainment & Promotion
                    </h3>

                    <p>
                        Artist promotion, branding, media exposure
                        and entertainment services.
                    </p>

                </div>

            </div>


            <div class="media-card">

                <img
                    src="E94E2B62-8DA5-4B74-B19C-E97D8F87F49C.jpeg"
                    alt="Big Shizzy">

                <div class="media-caption">

                    <h3>
                        Big Shizzy
                    </h3>

                    <p>
                        Artist • Entertainer • Creative
                    </p>

                </div>

            </div>


        </div>

    </div>

</section>


<!-- =====================================================
     CONTACT
===================================================== -->

<section class="contact" id="contact">

    <div class="container">

        <div class="contact-box">

            <h2>
                Let's Work Together
            </h2>

            <p>
                For bookings, collaborations, artist promotion,
                branding, events and other enquiries, get in touch.
            </p>


            <div class="contact-details">


                <div class="contact-item">

                    <strong>
                        WhatsApp
                    </strong>

                    <a
                        href="https://wa.me/2349070804147"
                        target="_blank"
                        rel="noopener">

                        +234 907 080 4147

                    </a>

                </div>


                <div class="contact-item">

                    <strong>
                        Email
                    </strong>

                    <a
                        href="mailto:adeshipe94@gmail.com">

                        adeshipe94@gmail.com

                    </a>

                </div>


            </div>


            <a
                class="btn btn-gold"
                href="https://wa.me/2349070804147?text=Hello%20Big%20Shizzy%2C%20I%20would%20like%20to%20make%20an%20enquiry."
                target="_blank"
                rel="noopener">

                Contact Big Shizzy

            </a>

        </div>

    </div>

</section>


<!-- =====================================================
     FOOTER
===================================================== -->

<footer>

    <div class="footer-logo">
        BIG SHIZZY
    </div>

    <p>
        © <span id="year"></span>
        Big Shizzy. All Rights Reserved.
    </p>

    <p>
        Artist • Entertainer • Creative
    </p>

</footer>


<!-- =====================================================
     JAVASCRIPT
===================================================== -->

<script>

/* Copyright year */

document.getElementById("year").textContent =
    new Date().getFullYear();


/* =====================================================
   PREVENT BROKEN IMAGE ICONS
===================================================== */

document.querySelectorAll("img").forEach(function(image) {

    image.addEventListener("error", function() {

        /*
         * Instead of displaying the ugly broken-image icon,
         * hide the failed image.
         */

        this.style.display = "none";

        /*
         * If this is the main hero image,
         * display our professional fallback.
         */

        if (this.classList.contains("hero-photo")) {

            const fallback =
                document.querySelector(".image-fallback");

            if (fallback) {
                fallback.style.display = "flex";
            }

        }

    });

});

</script>


</body>
</html>
