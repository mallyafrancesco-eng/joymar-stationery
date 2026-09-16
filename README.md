<!DOCTYPE html>
<html lang="sw">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>JOYMAR STATIONERY | Chunya - Ifumbo</title>

    <meta name="description" content="JOYMAR STATIONERY - Photocopy, Printing, Typing, Scanning, T-Shirt Printing, vifaa vya shule na ofisini. Ifumbo - Soko Jipya, Chunya.">

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            scroll-behavior: smooth;
        }

        body {
            font-family: Arial, Helvetica, sans-serif;
            background: #f5fff8;
            color: #173b27;
            line-height: 1.6;
        }

        /* HEADER */
        header {
            position: sticky;
            top: 0;
            z-index: 1000;
            background: #087f3e;
            box-shadow: 0 3px 15px rgba(0,0,0,0.15);
        }

        .navbar {
            max-width: 1150px;
            margin: auto;
            padding: 10px 20px;
            display: flex;
            align-items: center;
            justify-content: space-between;
        }

        .brand {
            display: flex;
            align-items: center;
            text-decoration: none;
            color: white;
        }

        .brand img {
            width: 58px;
            height: 58px;
            object-fit: contain;
            background: white;
            border-radius: 50%;
            padding: 3px;
            margin-right: 10px;
        }

        .brand-text {
            font-size: 21px;
            font-weight: bold;
            line-height: 1.1;
        }

        .brand-text span {
            display: block;
            color: #ffd500;
            font-size: 12px;
            letter-spacing: 2px;
            margin-top: 4px;
        }

        nav {
            display: flex;
            gap: 22px;
        }

        nav a {
            color: white;
            text-decoration: none;
            font-weight: bold;
            font-size: 15px;
            transition: 0.3s;
        }

        nav a:hover {
            color: #ffd500;
        }

        .menu-btn {
            display: none;
            border: none;
            background: #ffd500;
            color: #087f3e;
            font-size: 25px;
            padding: 5px 11px;
            border-radius: 7px;
            cursor: pointer;
        }

        /* HERO */
        .hero {
            min-height: 620px;
            display: flex;
            align-items: center;
            background:
                linear-gradient(rgba(0,105,50,0.88), rgba(0,105,50,0.88)),
                radial-gradient(circle at top right, #ffd500, transparent 35%);
            color: white;
            padding: 60px 20px;
        }

        .hero-content {
            max-width: 1150px;
            width: 100%;
            margin: auto;
            display: grid;
            grid-template-columns: 1.2fr 0.8fr;
            gap: 40px;
            align-items: center;
        }

        .hero h1 {
            font-size: 55px;
            line-height: 1.1;
            margin-bottom: 20px;
        }

        .hero h1 span {
            color: #ffd500;
        }

        .hero p {
            font-size: 19px;
            max-width: 650px;
            margin-bottom: 30px;
        }

        .hero-buttons {
            display: flex;
            gap: 15px;
            flex-wrap: wrap;
        }

        .btn {
            display: inline-block;
            text-decoration: none;
            padding: 14px 25px;
            border-radius: 30px;
            font-weight: bold;
            transition: 0.3s;
        }

        .btn-yellow {
            background: #ffd500;
            color: #075d2d;
        }

        .btn-yellow:hover {
            transform: translateY(-3px);
            background: #ffe45c;
        }

        .btn-outline {
            border: 2px solid white;
            color: white;
        }

        .btn-outline:hover {
            background: white;
            color: #087f3e;
        }

        .hero-logo {
            text-align: center;
        }

        .hero-logo img {
            width: 270px;
            height: 270px;
            object-fit: contain;
            background: white;
            border-radius: 50%;
            padding: 12px;
            box-shadow: 0 15px 40px rgba(0,0,0,0.25);
        }

        /* QUICK INFO */
        .quick-info {
            max-width: 1050px;
            margin: -45px auto 50px;
            position: relative;
            z-index: 5;
            background: white;
            border-radius: 18px;
            padding: 25px;
            box-shadow: 0 8px 30px rgba(0,0,0,0.12);
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 20px;
        }

        .quick-box {
            text-align: center;
            padding: 10px;
        }

        .quick-box .icon {
            font-size: 32px;
            margin-bottom: 8px;
        }

        .quick-box h3 {
            color: #087f3e;
            margin-bottom: 3px;
        }

        /* SECTIONS */
        section {
            padding: 70px 20px;
        }

        .container {
            max-width: 1150px;
            margin: auto;
        }

        .section-title {
            text-align: center;
            margin-bottom: 45px;
        }

        .section-title h2 {
            font-size: 36px;
            color: #087f3e;
            margin-bottom: 10px;
        }

        .section-title p {
            color: #55705f;
        }

        /* SERVICES */
        .services {
            background: white;
        }

        .service-grid {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 20px;
        }

        .service-card {
            background: #f5fff8;
            border: 1px solid #d9efdf;
            padding: 25px 18px;
            border-radius: 15px;
            text-align: center;
            transition: 0.3s;
        }

        .service-card:hover {
            transform: translateY(-7px);
            box-shadow: 0 10px 25px rgba(0,0,0,0.1);
            border-color: #ffd500;
        }

        .service-icon {
            width: 65px;
            height: 65px;
            margin: auto auto 15px;
            display: flex;
            align-items: center;
            justify-content: center;
            background: #087f3e;
            color: #ffd500;
            border-radius: 50%;
            font-size: 29px;
        }

        .service-card h3 {
            color: #087f3e;
            font-size: 17px;
            margin-bottom: 6px;
        }

        .service-card p {
            font-size: 14px;
            color: #607567;
        }

        /* ABOUT */
        .about {
            background: #effaf2;
        }

        .about-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 45px;
            align-items: center;
        }

        .about h2 {
            font-size: 36px;
            color: #087f3e;
            margin-bottom: 15px;
        }

        .about p {
            margin-bottom: 15px;
        }

        .about-list {
            list-style: none;
            margin-top: 20px;
        }

        .about-list li {
            margin-bottom: 12px;
            font-weight: bold;
        }

        .about-list li::before {
            content: "✓";
            color: #087f3e;
            background: #ffd500;
            border-radius: 50%;
            padding: 2px 6px;
            margin-right: 10px;
        }

        .about-box {
            background: #087f3e;
            color: white;
            border-radius: 20px;
            padding: 35px;
            text-align: center;
        }

        .about-box img {
            width: 150px;
            height: 150px;
            object-fit: contain;
            background: white;
            padding: 8px;
            border-radius: 50%;
            margin-bottom: 15px;
        }

        .about-box h3 {
            color: #ffd500;
            font-size: 27px;
        }

        /* ORDER */
        .order {
            background: white;
        }

        .order-box {
            max-width: 750px;
            margin: auto;
            background: #f5fff8;
            padding: 35px;
            border-radius: 20px;
            box-shadow: 0 8px 25px rgba(0,0,0,0.08);
        }

        .form-group {
            margin-bottom: 18px;
        }

        .form-group label {
            display: block;
            font-weight: bold;
            margin-bottom: 7px;
            color: #087f3e;
        }

        input,
        select,
        textarea {
            width: 100%;
            padding: 13px;
            border: 1px solid #c8dfcf;
            border-radius: 9px;
            font-size: 15px;
            outline: none;
            background: white;
        }

        input:focus,
        select:focus,
        textarea:focus {
            border-color: #087f3e;
        }

        textarea {
            min-height: 120px;
            resize: vertical;
        }

        .submit-btn {
            width: 100%;
            border: none;
            cursor: pointer;
            background: #087f3e;
            color: white;
            padding: 15px;
            border-radius: 30px;
            font-size: 16px;
            font-weight: bold;
        }

        .submit-btn:hover {
            background: #05632f;
        }

        /* CONTACT */
        .contact {
            background: #087f3e;
            color: white;
        }

        .contact .section-title h2 {
            color: #ffd500;
        }

        .contact .section-title p {
            color: white;
        }

        .contact-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 20px;
        }

        .contact-card {
            background: rgba(255,255,255,0.1);
            padding: 30px 20px;
            border-radius: 15px;
            text-align: center;
        }

        .contact-card .icon {
            font-size: 35px;
            margin-bottom: 10px;
        }

        .contact-card h3 {
            color: #ffd500;
            margin-bottom: 7px;
        }

        .contact-card a {
            color: white;
            text-decoration: none;
            font-weight: bold;
        }

        .whatsapp-contact {
            display: inline-block;
            margin-top: 30px;
            background: #ffd500;
            color: #075d2d !important;
            padding: 13px 25px;
            border-radius: 30px;
        }

        /* FOOTER */
        footer {
            background: #043d1d;
            color: white;
            text-align: center;
            padding: 25px 15px;
        }

        footer strong {
            color: #ffd500;
        }

        /* FLOATING WHATSAPP */
        .floating-whatsapp {
            position: fixed;
            right: 20px;
            bottom: 20px;
            width: 60px;
            height: 60px;
            background: #25D366;
            color: white;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            text-decoration: none;
            font-size: 30px;
            box-shadow: 0 5px 20px rgba(0,0,0,0.25);
            z-index: 999;
            animation: pulse 2s infinite;
        }

        @keyframes pulse {
            0% {
                transform: scale(1);
            }

            50% {
                transform: scale(1.08);
            }

            100% {
                transform: scale(1);
            }
        }

        /* MOBILE */
        @media (max-width: 850px) {

            nav {
                display: none;
                position: absolute;
                top: 78px;
                left: 0;
                width: 100%;
                background: #087f3e;
                flex-direction: column;
                gap: 0;
                padding: 10px 20px 20px;
            }

            nav.active {
                display: flex;
            }

            nav a {
                padding: 13px 5px;
                border-bottom: 1px solid rgba(255,255,255,0.15);
            }

            .menu-btn {
                display: block;
            }

            .hero {
                min-height: auto;
                padding: 55px 20px 80px;
            }

            .hero-content {
                grid-template-columns: 1fr;
                text-align: center;
            }

            .hero h1 {
                font-size: 40px;
            }

            .hero p {
                font-size: 16px;
            }

            .hero-buttons {
                justify-content: center;
            }

            .hero-logo {
                order: -1;
            }

            .hero-logo img {
                width: 190px;
                height: 190px;
            }

            .quick-info {
                margin: -30px 15px 20px;
                grid-template-columns: 1fr;
            }

            section {
                padding: 55px 15px;
            }

            .section-title h2 {
                font-size: 30px;
            }

            .service-grid {
                grid-template-columns: repeat(2, 1fr);
                gap: 13px;
            }

            .service-card {
                padding: 20px 10px;
            }

            .service-icon {
                width: 55px;
                height: 55px;
                font-size: 24px;
            }

            .about-grid {
                grid-template-columns: 1fr;
                gap: 25px;
            }

            .about h2 {
                font-size: 30px;
            }

            .contact-grid {
                grid-template-columns: 1fr;
            }

            .order-box {
                padding: 22px 17px;
            }
        }

        @media (max-width: 430px) {

            .brand img {
                width: 50px;
                height: 50px;
            }

            .brand-text {
                font-size: 17px;
            }

            .hero h1 {
                font-size: 34px;
            }

            .service-grid {
                grid-template-columns: 1fr 1fr;
            }

            .service-card h3 {
                font-size: 15px;
            }

            .service-card p {
                font-size: 12px;
            }
        }
    </style>
</head>

<body>

    <!-- HEADER -->
    <header>
        <div class="navbar">

            <a href="#home" class="brand">
                <img src="logo.jpg" alt="JOYMAR STATIONERY Logo">

                <div class="brand-text">
                    JOYMAR
                    <span>STATIONERY</span>
                </div>
            </a>

            <button class="menu-btn" onclick="toggleMenu()">☰</button>

            <nav id="navMenu">
                <a href="#home" onclick="closeMenu()">Home</a>
                <a href="#huduma" onclick="closeMenu()">Huduma</a>
                <a href="#kuhusu" onclick="closeMenu()">Kuhusu</a>
                <a href="#agiza" onclick="closeMenu()">Agiza</a>
                <a href="#mawasiliano" onclick="closeMenu()">Mawasiliano</a>
            </nav>

        </div>
    </header>


    <!-- HERO -->
    <section class="hero" id="home">

        <div class="hero-content">

            <div>
                <h1>
                    Karibu <span>JOYMAR</span> STATIONERY
                </h1>

                <p>
                    Tunakupa huduma mbalimbali za uchapishaji,
                    stationery na huduma za kidigitali kwa ubora
                    na uaminifu.
                </p>

                <div class="hero-buttons">
                    <a href="#huduma" class="btn btn-yellow">
                        Tazama Huduma
                    </a>

                    <a href="https://wa.me/255765553405?text=Habari%20JOYMAR%20STATIONERY,%20nahitaji%20huduma." 
                       class="btn btn-outline"
                       target="_blank">
                        💬 WhatsApp
                    </a>
                </div>
            </div>

            <div class="hero-logo">
                <img src="logo.jpg" alt="JOYMAR STATIONERY">
            </div>

        </div>

    </section>


    <!-- QUICK INFO -->
    <div class="quick-info">

        <div class="quick-box">
            <div class="icon">📍</div>
            <h3>Mahali Tulipo</h3>
            <p>Ifumbo - Soko Jipya, Chunya</p>
        </div>

        <div class="quick-box">
            <div class="icon">📞</div>
            <h3>Wasiliana Nasi</h3>
            <p>0765 553 405</p>
        </div>

        <div class="quick-box">
            <div class="icon">🖨️</div>
            <h3>Huduma</h3>
            <p>Printing & Stationery</p>
        </div>

    </div>


    <!-- SERVICES -->
    <section class="services" id="huduma">

        <div class="container">

            <div class="section-title">
                <h2>Huduma Zetu</h2>
                <p>Huduma mbalimbali zinazopatikana JOYMAR STATIONERY</p>
            </div>

            <div class="service-grid">

                <div class="service-card">
                    <div class="service-icon">📄</div>
                    <h3>Photocopy</h3>
                    <p>Huduma za photocopy za nyaraka mbalimbali.</p>
                </div>

                <div class="service-card">
                    <div class="service-icon">🖨️</div>
                    <h3>Printing</h3>
                    <p>Kuprint nyaraka na documents mbalimbali.</p>
                </div>

                <div class="service-card">
                    <div class="service-icon">⌨️</div>
                    <h3>Typing</h3>
                    <p>Kuandika na kuandaa documents.</p>
                </div>

                <div class="service-card">
                    <div class="service-icon">📑</div>
                    <h3>Scanning</h3>
                    <p>Scanning ya nyaraka mbalimbali.</p>
                </div>

                <div class="service-card">
                    <div class="service-icon">👶</div>
                    <h3>Vyeti vya Kuzaliwa</h3>
                    <p>Huduma zinazohusiana na vyeti vya kuzaliwa.</p>
                </div>

                <div class="service-card">
                    <div class="service-icon">📜</div>
                    <h3>Cheti cha Kifo</h3>
                    <p>Huduma zinazohusiana na cheti cha kifo.</p>
                </div>

                <div class="service-card">
                    <div class="service-icon">💌</div>
                    <h3>Kadi za Sherehe</h3>
                    <p>Kadi kwa ajili ya sherehe mbalimbali.</p>
                </div>

                <div class="service-card">
                    <div class="service-icon">🏥</div>
                    <h3>Kadi za Kliniki</h3>
                    <p>Huduma za uchapishaji wa kadi za kliniki.</p>
                </div>

                <div class="service-card">
                    <div class="service-icon">👕</div>
                    <h3>T-Shirt Printing</h3>
                    <p>Kuprint design kwenye T-Shirt.</p>
                </div>

                <div class="service-card">
                    <div class="service-icon">☕</div>
                    <h3>Kuprint Vikombe</h3>
                    <p>Uchapishaji kwenye vikombe.</p>
                </div>

                <div class="service-card">
                    <div class="service-icon">🍽️</div>
                    <h3>Kuprint Sahani</h3>
                    <p>Uchapishaji kwenye sahani.</p>
                </div>

                <div class="service-card">
                    <div class="service-icon">🧢</div>
                    <h3>Kuprint Kofia</h3>
                    <p>Uchapishaji kwenye kofia.</p>
                </div>

                <div class="service-card">
                    <div class="service-icon">🏢</div>
                    <h3>Vifaa vya Ofisini</h3>
                    <p>Vifaa mbalimbali kwa matumizi ya ofisi.</p>
                </div>

                <div class="service-card">
                    <div class="service-icon">🎒</div>
                    <h3>Vifaa vya Shuleni</h3>
                    <p>Vifaa mbalimbali vya shule.</p>
                </div>

            </div>

        </div>

    </section>


    <!-- ABOUT -->
    <section class="about" id="kuhusu">

        <div class="container">

            <div class="about-grid">

                <div>
                    <h2>Kuhusu JOYMAR STATIONERY</h2>

                    <p>
                        JOYMAR STATIONERY ni kituo kinachotoa
                        huduma mbalimbali za stationery,
                        printing na uchapishaji.
                    </p>

                    <p>
                        Tunapatikana <strong>Ifumbo - Soko Jipya,
                        Chunya</strong>, kwa ajili ya kukuhudumia
                        wewe, wanafunzi, wafanyabiashara na taasisi.
                    </p>

                    <ul class="about-list">
                        <li>Huduma mbalimbali sehemu moja</li>
                        <li>Uchapishaji wa aina mbalimbali</li>
                        <li>Huduma za stationery</li>
                        <li>Maagizo kupitia WhatsApp</li>
                    </ul>
                </div>

                <div class="about-box">

                    <img src="logo.jpg" alt="JOYMAR STATIONERY Logo">

                    <h3>JOYMAR STATIONERY</h3>

                    <p>
                        Ifumbo - Soko Jipya, Chunya
                    </p>

                </div>

            </div>

        </div>

    </section>


    <!-- ORDER -->
    <section class="order" id="agiza">

        <div class="container">

            <div class="section-title">
                <h2>Agiza Huduma</h2>
                <p>
                    Jaza taarifa zako. Tutakupokea kupitia WhatsApp.
                </p>
            </div>

            <div class="order-box">

                <form onsubmit="sendWhatsApp(event)">

                    <div class="form-group">
                        <label for="name">Jina lako</label>
                        <input
                            type="text"
                            id="name"
                            placeholder="Andika jina lako"
                            required>
                    </div>

                    <div class="form-group">
                        <label for="phone">Namba ya simu</label>
                        <input
                            type="tel"
                            id="phone"
                            placeholder="Mfano: 0712 345 678"
                            required>
                    </div>

                    <div class="form-group">
                        <label for="service">Chagua huduma</label>

                        <select id="service" required>

                            <option value="">-- Chagua huduma --</option>

                            <option>Photocopy</option>
                            <option>Printing</option>
                            <option>Typing</option>
                            <option>Scanning</option>
                            <option>Vyeti vya kuzaliwa</option>
                            <option>Cheti cha kifo</option>
                            <option>Kadi za sherehe</option>
                            <option>Kadi za kliniki</option>
                            <option>Kuprint T-Shirt</option>
                            <option>Kuprint vikombe</option>
                            <option>Kuprint sahani</option>
                            <option>Kuprint kofia</option>
                            <option>Vifaa vya ofisini</option>
                            <option>Vifaa vya shuleni</option>

                        </select>
                    </div>

                    <div class="form-group">
                        <label for="message">Maelezo ya oda</label>

                        <textarea
                            id="message"
                            placeholder="Andika maelezo ya huduma unayohitaji..."
                            required></textarea>
                    </div>

                    <button type="submit" class="submit-btn">
                        💬 Tuma Oda WhatsApp
                    </button>

                </form>

            </div>

        </div>

    </section>


    <!-- CONTACT -->
    <section class="contact" id="mawasiliano">

        <div class="container">

            <div class="section-title">
                <h2>Wasiliana Nasi</h2>
                <p>
                    Tunapatikana tayari kukuhudumia.
                </p>
            </div>

            <div class="contact-grid">

                <div class="contact-card">
                    <div class="icon">📍</div>
                    <h3>Mahali</h3>
                    <p>Ifumbo - Soko Jipya</p>
                    <p>Chunya, Tanzania</p>
                </div>

                <div class="contact-card">
                    <div class="icon">📞</div>
                    <h3>Simu</h3>
                    <p>
                        <a href="tel:0765553405">
                            0765 553 405
                        </a>
                    </p>

                    <p>
                        <a href="tel:0675102636">
                            0675 102 636
                        </a>
                    </p>
                </div>

                <div class="contact-card">
                    <div class="icon">💬</div>
                    <h3>WhatsApp</h3>
                    <p>
                        <a href="https://wa.me/255765553405"
                           target="_blank">
                            0765 553 405
                        </a>
                    </p>
                </div>

            </div>

            <div style="text-align:center;">
                <a
                    class="whatsapp-contact"
                    href="https://wa.me/255765553405?text=Habari%20JOYMAR%20STATIONERY,%20nahitaji%20huduma."
                    target="_blank">
                    💬 Chat nasi WhatsApp
                </a>
            </div>

        </div>

    </section>


    <!-- FOOTER -->
    <footer>

        <p>
            © 2026 <strong>JOYMAR STATIONERY</strong>.
            Haki zote zimehifadhiwa.
        </p>

        <p>
            Ifumbo - Soko Jipya, Chunya
        </p>

    </footer>


    <!-- FLOATING WHATSAPP -->
    <a
        class="floating-whatsapp"
        href="https://wa.me/255765553405?text=Habari%20JOYMAR%20STATIONERY,%20nahitaji%20huduma."
        target="_blank"
        aria-label="WhatsApp">
        💬
    </a>


    <script>

        /* MOBILE MENU */

        function toggleMenu() {
            document.getElementById("navMenu").classList.toggle("active");
        }

        function closeMenu() {
            document.getElementById("navMenu").classList.remove("active");
        }


        /* WHATSAPP ORDER */

        function sendWhatsApp(event) {

            event.preventDefault();

            const name =
                document.getElementById("name").value;

            const phone =
                document.getElementById("phone").value;

            const service =
                document.getElementById("service").value;

            const message =
                document.getElementById("message").value;

            const whatsappMessage =
                "Habari JOYMAR STATIONERY,%0A%0A" +
                "Naitwa: " + encodeURIComponent(name) +
                "%0A" +
                "Namba yangu: " + encodeURIComponent(phone) +
                "%0A" +
                "Huduma ninayohitaji: " +
                encodeURIComponent(service) +
                "%0A" +
                "Maelezo: " +
                encodeURIComponent(message);

            const whatsappURL =
                "https://wa.me/255765553405?text=" +
                whatsappMessage;

            window.open(whatsappURL, "_blank");
        }

    </script>

</body>
</html>
