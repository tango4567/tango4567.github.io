<!DOCTYPE html>
<html lang="hi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>पूज्या किशोरी साक्षी दीदी - अंतर्राष्ट्रीय कथावाचिका</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            background: linear-gradient(to bottom, #fff5e6, #ffe6cc);
        }

        /* Header */
        header {
            background: linear-gradient(to right, #e67e22, #c0392b);
            color: white;
            padding: 20px 0;
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        .header-content {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
        }

        .header-title h1 {
            font-size: 2.5em;
            margin-bottom: 5px;
        }

        .header-title p {
            font-size: 1.1em;
            color: #ffe6cc;
        }

        nav {
            display: flex;
            gap: 30px;
            flex-wrap: wrap;
        }

        nav a {
            color: white;
            text-decoration: none;
            font-size: 1.1em;
            transition: color 0.3s;
            padding: 5px 10px;
        }

        nav a:hover {
            color: #ffd966;
        }

        /* Hero Section */
        .hero {
            max-width: 1200px;
            margin: 40px auto;
            padding: 0 20px;
        }

        .hero-card {
            background: white;
            border-radius: 20px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.2);
            overflow: hidden;
        }

        .hero-header {
            background: linear-gradient(to right, #ffd966, #e67e22);
            padding: 40px;
            text-align: center;
        }

        .hero-header h2 {
            font-size: 3em;
            color: white;
            margin-bottom: 10px;
        }

        .hero-header p {
            font-size: 1.5em;
            color: white;
        }

        .hero-content {
            padding: 40px;
        }

        .hero-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }

        .katha-list {
            background: linear-gradient(to bottom right, #ffe6cc, #ffcccc);
            padding: 30px;
            border-radius: 15px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }

        .katha-list h3 {
            color: #c0392b;
            font-size: 1.8em;
            margin-bottom: 20px;
        }

        .katha-list ul {
            list-style: none;
        }

        .katha-list li {
            padding: 10px 0;
            border-bottom: 1px solid #e67e22;
            color: #333;
            font-size: 1.1em;
        }

        .katha-list li:last-child {
            border-bottom: none;
        }

        .info-boxes {
            display: flex;
            flex-direction: column;
            gap: 20px;
        }

        .info-box {
            padding: 25px;
            border-radius: 15px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }

        .info-box.location {
            background: linear-gradient(to bottom right, #fff4e6, #ffe6cc);
        }

        .info-box.specialty {
            background: linear-gradient(to bottom right, #ffcccc, #ffb3b3);
        }

        .info-box.quote {
            background: linear-gradient(to bottom right, #ffcc99, #ff9966);
            text-align: center;
            font-style: italic;
            font-size: 1.2em;
            color: #333;
        }

        .info-box h4 {
            font-size: 1.3em;
            margin-bottom: 10px;
            color: #c0392b;
        }

        /* About Section */
        .about {
            max-width: 1000px;
            margin: 60px auto;
            padding: 0 20px;
        }

        .about-card {
            background: white;
            border-radius: 20px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.2);
            padding: 50px;
        }

        .about-card h2 {
            color: #e67e22;
            font-size: 2.5em;
            text-align: center;
            margin-bottom: 30px;
        }

        .about-card p {
            font-size: 1.2em;
            color: #555;
            margin-bottom: 20px;
            text-align: justify;
        }

        .features {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
            margin-top: 40px;
        }

        .feature-box {
            padding: 30px;
            border-radius: 15px;
            text-align: center;
        }

        .feature-box.orange {
            background: #ffe6cc;
        }

        .feature-box.red {
            background: #ffcccc;
        }

        .feature-box.yellow {
            background: #fff4cc;
        }

        .feature-icon {
            font-size: 3em;
            margin-bottom: 15px;
        }

        .feature-box h3 {
            font-size: 1.5em;
            margin-bottom: 10px;
            color: #c0392b;
        }

        /* Services Section */
        .services {
            max-width: 1200px;
            margin: 60px auto;
            padding: 0 20px;
        }

        .services h2 {
            color: #e67e22;
            font-size: 2.5em;
            text-align: center;
            margin-bottom: 40px;
        }

        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 30px;
        }

        .service-card {
            background: white;
            padding: 35px;
            border-radius: 15px;
            box-shadow: 0 5px 20px rgba(0,0,0,0.15);
            transition: transform 0.3s, box-shadow 0.3s;
        }

        .service-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 10px 30px rgba(0,0,0,0.25);
        }

        .service-card .icon {
            font-size: 3.5em;
            margin-bottom: 15px;
        }

        .service-card h3 {
            color: #e67e22;
            font-size: 1.6em;
            margin-bottom: 15px;
        }

        .service-card p {
            color: #666;
            font-size: 1.1em;
        }

        /* Contact Section */
        .contact {
            max-width: 1000px;
            margin: 60px auto;
            padding: 0 20px;
        }

        .contact-card {
            background: white;
            border-radius: 20px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.2);
            padding: 50px;
        }

        .contact-card h2 {
            color: #e67e22;
            font-size: 2.5em;
            text-align: center;
            margin-bottom: 40px;
        }

        .contact-info {
            display: flex;
            flex-direction: column;
            gap: 25px;
        }

        .contact-item {
            display: flex;
            align-items: center;
            gap: 20px;
            padding: 25px;
            border-radius: 15px;
        }

        .contact-item.phone {
            background: #ffe6cc;
        }

        .contact-item.location {
            background: #ffcccc;
        }

        .contact-item.social {
            background: #fff4e6;
        }

        .contact-icon {
            font-size: 2.5em;
        }

        .contact-details h3 {
            font-size: 1.5em;
            color: #c0392b;
            margin-bottom: 8px;
        }

        .contact-details p {
            font-size: 1.1em;
            color: #555;
        }

        .social-links {
            display: flex;
            gap: 20px;
            margin-top: 15px;
        }

        .social-link {
            padding: 10px 20px;
            border-radius: 8px;
            text-decoration: none;
            color: white;
            font-weight: bold;
            transition: transform 0.3s;
        }

        .social-link:hover {
            transform: scale(1.05);
        }

        .youtube {
            background: #ff0000;
        }

        .facebook {
            background: #1877f2;
        }

        .instagram {
            background: #e4405f;
        }

        .booking-box {
            background: linear-gradient(to right, #ffe6cc, #ffcccc);
            padding: 30px;
            border-radius: 15px;
            text-align: center;
            margin-top: 30px;
        }

        .booking-icon {
            font-size: 3em;
            margin-bottom: 15px;
        }

        .booking-box h3 {
            font-size: 1.8em;
            color: #c0392b;
            margin-bottom: 10px;
        }

        .booking-box p {
            font-size: 1.2em;
            color: #555;
        }

        /* Footer */
        footer {
            background: linear-gradient(to right, #c0392b, #e67e22);
            color: white;
            text-align: center;
            padding: 30px 20px;
            margin-top: 60px;
        }

        footer p {
            font-size: 1.2em;
            margin: 10px 0;
        }

        /* Responsive */
        @media (max-width: 768px) {
            .header-content {
                flex-direction: column;
                text-align: center;
            }

            .header-title h1 {
                font-size: 1.8em;
            }

            nav {
                margin-top: 15px;
                justify-content: center;
            }

            .hero-header h2 {
                font-size: 2em;
            }

            .hero-content {
                padding: 20px;
            }

            .about-card, .contact-card {
                padding: 30px 20px;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <div class="header-content">
            <div class="header-title">
                <h1>पूज्या किशोरी साक्षी दीदी</h1>
                <p>अंतर्राष्ट्रीय कथावाचिका</p>
            </div>
            <nav>
                <a href="#home">होम</a>
                <a href="#about">परिचय</a>
                <a href="#services">सेवाएं</a>
                <a href="#contact">संपर्क</a>
            </nav>
        </div>
    </header>

    <!-- Hero Section -->
    <section id="home" class="hero">
        <div class="hero-card">
            <div class="hero-header">
                <h2>🙏 स्वागत है 🙏</h2>
                <p>पूज्या किशोरी साक्षी दीदी के आध्यात्मिक संसार में</p>
            </div>
            <div class="hero-content">
                <div class="hero-grid">
                    <div class="katha-list">
                        <h3>कथा विशेषज्ञता</h3>
                        <ul>
                            <li>📖 श्रीमद् भागवत कथा</li>
                            <li>📖 श्रीराम कथा</li>
                            <li>📖 देवी भागवत पुराण</li>
                            <li>📖 शिव पुराण</li>
                            <li>📖 नर्मदा पुराण</li>
                            <li>📖 नानी बाई का मायरा</li>
                        </ul>
                    </div>
                    <div class="info-boxes">
                        <div class="info-box location">
                            <h4>📍 स्थान</h4>
                            <p>जबलपुर (म.प.)<br>श्रीधाम वृन्दावन (उ.प.)</p>
                        </div>
                        <div class="info-box specialty">
                            <h4>🏆 विशेषता</h4>
                            <p>अंतर्राष्ट्रीय स्तर की प्रसिद्ध कथावाचिका</p>
                        </div>
                        <div class="info-box quote">
                            <p>"धर्म और आध्यात्मिकता के प्रचार-प्रसार में समर्पित"</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="about">
        <div class="about-card">
            <h2>परिचय</h2>
            <p>
                पूज्या किशोरी साक्षी दीदी एक प्रसिद्ध अंतर्राष्ट्रीय कथावाचिका हैं जो भारतीय धार्मिक और आध्यात्मिक परंपराओं को जन-जन तक पहुंचाने में समर्पित हैं।
            </p>
            <p>
                जबलपुर (मध्य प्रदेश) और श्रीधाम वृन्दावन (उत्तर प्रदेश) में स्थित, दीदी जी विभिन्न पुराणों और धार्मिक ग्रंथों की गहन व्याख्या करती हैं। उनकी कथाओं में भक्ति, ज्ञान और आध्यात्मिकता का अद्भुत संगम होता है।
            </p>
            <div class="features">
                <div class="feature-box orange">
                    <div class="feature-icon">📚</div>
                    <h3>कथा विशेषज्ञ</h3>
                    <p>विभिन्न पुराणों की विशेषज्ञता</p>
                </div>
                <div class="feature-box red">
                    <div class="feature-icon">👥</div>
                    <h3>जन सेवा</h3>
                    <p>हजारों श्रद्धालुओं को प्रेरित</p>
                </div>
                <div class="feature-box yellow">
                    <div class="feature-icon">🏆</div>
                    <h3>प्रसिद्धि</h3>
                    <p>अंतर्राष्ट्रीय मान्यता प्राप्त</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section id="services" class="services">
        <h2>हमारी सेवाएं</h2>
        <div class="services-grid">
            <div class="service-card">
                <div class="icon">📚</div>
                <h3>कथा आयोजन</h3>
                <p>विभिन्न धार्मिक कथाओं का आयोजन और संचालन</p>
            </div>
            <div class="service-card">
                <div class="icon">🕉️</div>
                <h3>आध्यात्मिक परामर्श</h3>
                <p>व्यक्तिगत और सामूहिक आध्यात्मिक मार्गदर्शन</p>
            </div>
            <div class="service-card">
                <div class="icon">🙏</div>
                <h3>धार्मिक समारोह</h3>
                <p>विशेष धार्मिक अवसरों पर कथा वाचन</p>
            </div>
            <div class="service-card">
                <div class="icon">💻</div>
                <h3>ऑनलाइन प्रवचन</h3>
                <p>ऑनलाइन माध्यम से कथा प्रसारण</p>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="contact">
        <div class="contact-card">
            <h2>संपर्क करें</h2>
            <div class="contact-info">
                <div class="contact-item phone">
                    <div class="contact-icon">📱</div>
                    <div class="contact-details">
                        <h3>मोबाइल नंबर</h3>
                        <p>7000574916, 9329843665</p>
                    </div>
                </div>
                
                <div class="contact-item location">
                    <div class="contact-icon">📍</div>
                    <div class="contact-details">
                        <h3>पता</h3>
                        <p>जबलपुर, मध्य प्रदेश<br>
                        श्रीधाम वृन्दावन, उत्तर प्रदेश</p>
                    </div>
                </div>

                <div class="contact-item social">
                    <div class="contact-icon">📲</div>
                    <div class="contact-details">
                        <h3>सोशल मीडिया</h3>
                        <div class="social-links">
                            <a href="#" class="social-link youtube">YouTube</a>
                            <a href="#" class="social-link facebook">Facebook</a>
                            <a href="#" class="social-link instagram">Instagram</a>
                        </div>
                    </div>
                </div>
            </div>

            <div class="booking-box">
                <div class="booking-icon">📅</div>
                <h3>कथा आयोजन के लिए</h3>
                <p>कृपया उपरोक्त नंबर पर संपर्क करें</p>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <p>🙏 जय श्री कृष्ण 🙏</p>
        <p>पूज्या किशोरी साक्षी दीदी - अंतर्राष्ट्रीय कथावाचिका</p>
        <p style="font-size: 0.9em; margin-top: 15px;">© 2024 All Rights Reserved</p>
    </footer>
</body>
</html>
