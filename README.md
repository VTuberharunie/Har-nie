
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HARŪNIE VTuber Group</title>
    <style>
        /* General Styles */
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            background: linear-gradient(135deg, #1a1a1a, #2c3e50);
            color: #fff;
        }

        .container {
            width: 90%;
            margin: auto;
            max-width: 1200px;
        }

        /* Header Styles */
        header {
            background: rgba(0, 0, 0, 0.7);
            padding: 20px 0;
            text-align: center;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.3);
        }

        .logo-container img {
            height: 150px;
            transition: transform 0.3s ease;
        }

        .logo-container img:hover {
            transform: scale(1.1);
        }

        /* Navigation Styles */
        nav {
            background: rgba(0, 0, 0, 0.8);
            padding: 10px 0;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.3);
        }

        nav ul {
            list-style-type: none;
            padding: 0;
            text-align: center;
        }

        nav ul li {
            display: inline;
            margin: 0 15px;
        }

        nav ul li a {
            color: #fff;
            text-decoration: none;
            font-weight: bold;
            transition: color 0.3s ease;
        }

        nav ul li a:hover {
            color: #ff6f61;
        }

        /* Hero Section */
        .hero {
            text-align: center;
            padding: 100px 0;
            background: rgba(0, 0, 0, 0.5);
            margin-bottom: 40px;
        }

        .hero h1 {
            font-size: 3rem;
            margin-bottom: 20px;
            animation: fadeIn 2s ease-in-out;
        }

        .hero p {
            font-size: 1.2rem;
            animation: fadeIn 3s ease-in-out;
        }

        /* VTuber Cards */
        .vtubers-grid {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 20px;
        }

        .vtuber-card {
            background: rgba(255, 255, 255, 0.1);
            border-radius: 15px;
            padding: 20px;
            width: 30%;
            text-align: center;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .vtuber-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.3);
        }

        .vtuber-image {
            max-width: 100%;
            border-radius: 10px;
            margin-bottom: 15px;
        }

        .vtuber-name {
            font-size: 1.5rem;
            margin-bottom: 10px;
        }

        .vtuber-role {
            font-size: 1rem;
            color: #ff6f61;
            margin-bottom: 10px;
        }

        .vtuber-description {
            font-size: 0.9rem;
            margin-bottom: 15px;
        }

        .social-links img {
            width: 25px;
            margin: 0 5px;
            transition: transform 0.3s ease;
        }

        .social-links img:hover {
            transform: scale(1.2);
        }

        /* Schedule Section */
        .schedule {
            background: rgba(0, 0, 0, 0.5);
            padding: 40px 20px;
            border-radius: 15px;
            margin: 40px 0;
        }

        .schedule-title {
            text-align: center;
            font-size: 2rem;
            margin-bottom: 20px;
        }

        /* Desktop Schedule */
        .desktop-schedule {
            display: grid;
            grid-template-columns: repeat(7, 1fr);
            gap: 10px;
            text-align: center;
        }

        .desktop-schedule .day {
            background: rgba(255, 255, 255, 0.1);
            padding: 10px;
            border-radius: 10px;
        }

        .desktop-schedule .day h3 {
            margin: 0 0 10px 0;
            font-size: 1.2rem;
        }

        .desktop-schedule .day p {
            margin: 0;
            font-size: 0.9rem;
        }

        /* Mobile Schedule */
        .mobile-schedule {
            display: none;
        }

        .mobile-schedule .vtuber-schedule {
            background: rgba(255, 255, 255, 0.1);
            padding: 15px;
            border-radius: 10px;
            margin-bottom: 10px;
            cursor: pointer;
            transition: background 0.3s ease;
        }

        .mobile-schedule .vtuber-schedule:hover {
            background: rgba(255, 255, 255, 0.2);
        }

        .mobile-schedule .vtuber-schedule h3 {
            margin: 0 0 10px 0;
            font-size: 1.2rem;
        }

        .mobile-schedule .vtuber-schedule p {
            margin: 0;
            font-size: 0.9rem;
            display: none;
        }

        .mobile-schedule .vtuber-schedule.active p {
            display: block;
        }

        /* Footer Styles */
        footer {
            background: rgba(0, 0, 0, 0.8);
            padding: 20px 0;
            text-align: center;
            margin-top: 40px;
            box-shadow: 0 -4px 10px rgba(0, 0, 0, 0.3);
        }

        footer p {
            margin: 0;
            font-size: 0.9rem;
        }

        /* Animations */
        @keyframes fadeIn {
            from {
                opacity: 0;
            }
            to {
                opacity: 1;
            }
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .vtuber-card {
                width: 100%;
            }

            .desktop-schedule {
                display: none;
            }

            .mobile-schedule {
                display: block;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="logo-container">
            <img src="https://cdn.discordapp.com/attachments/812966246806192128/1350186993019261088/HARUNIE_1.png?ex=67d5d320&is=67d481a0&hm=88ee16f82aecd510b053a23b30c7a64b8236c4ee3936d7a138f81ed5816c169c&" alt="Harunie Logo">
        </div>
    </header>

    <nav>
        <div class="container">
            <ul class="menu">
                <li><a href="#home">Home</a></li>
                <li><a href="#vtubers">VTubers</a></li>
                <li><a href="#content">Content</a></li>
                <li><a href="#schedule">Schedule</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </div>
    </nav>

    <section class="hero" id="home">
        <div class="container">
            <h1>Welcome to HARŪNIE Community</h1>
            <p>Discover our amazing virtual talents bringing joy and entertainment to fans worldwide!</p>
        </div>
    </section>

    <main class="container">
        <section id="vtubers">
            <h2 class="section-title">Our Talents</h2>
            <div class="vtubers-grid">
                <!-- VTuber 1 -->
                <div class="vtuber-card">
                    <img src="https://cdn.discordapp.com/attachments/812966246806192128/1350208575179587735/IMG_1094.png?ex=67d5e739&is=67d495b9&hm=ef457c0aba708a40f68f8365113122754da8e86a30287d9c8e83c2aee077c57a&" alt="Ryuga Ranjaya" class="vtuber-image">
                    <div class="vtuber-info">
                        <h3 class="vtuber-name">Ryuga Ranjaya</h3>
                        <div class="vtuber-role">VTuber / Gamer</div>
                        <p class="vtuber-description">Ryuga Ranjaya is the Spirit Wolf King tasked with maintaining the balance of the world.</p>
                        <div class="social-links">
                            <a href="https://youtube.com/@ryugaranjaya?si=P5IptDy9svmC4Gyx"><img src="https://cdn.discordapp.com/attachments/812966246806192128/1350193854057283695/4.png?ex=67d5d984&is=67d48804&hm=6cc8ceaf475441439b6057278bf381c67066eaf82cf73d258b1308949eeba1db&" alt="YouTube"></a>
                            <a href="https://twitter.com/RyugaRanjayaa?t=MiGvSFFbUYrJTBBUf4F5FQ&s=09"><img src="https://cdn.discordapp.com/attachments/812966246806192128/1350193853226946593/2.png?ex=67d5d983&is=67d48803&hm=81ad7a1a422f41d87d067d5e5a7125a16201e8cfde1bf625f01573fa0993256c&" alt="Twitter"></a>
                            <a href="https://www.instagram.com/ryugaranjaya"><img src="https://cdn.discordapp.com/attachments/812966246806192128/1350193853696835624/3.png?ex=67d5d984&is=67d48804&hm=411e0a8a5a76e1787b5d318afb0cba7f9cd6aa62018b79f16d918b40e6e690ea&" alt="Instagram"></a>
                            <a href="https://www.tiktok.com/@ryugaranjaya"><img src="https://cdn.discordapp.com/attachments/812966246806192128/1350193854413930557/5.png?ex=67d5d984&is=67d48804&hm=971b461097ad8fba1e4a681d65b4b6c56a50420355264313d98f5914b98bb006&" alt="TikTok"></a>
                        </div>
                    </div>
                </div>

                <!-- VTuber 2 -->
                <div class="vtuber-card">
                    <img src="https://cdn.discordapp.com/attachments/812966246806192128/1350208620062576700/Naana_milktea.png?ex=67d5e744&is=67d495c4&hm=b8aa0d6cd765aecb4521b328d0f990a253dd2185df51e32a644a2a14d6d91981&" alt="Kokona Naana" class="vtuber-image">
                    <div class="vtuber-info">
                        <h3 class="vtuber-name">Kokona Naana</h3>
                        <div class="vtuber-role">VTuber / Gamer</div>
                        <p class="vtuber-description">An ordinary college student.</p>
                        <div class="social-links">
                            <a href="https://www.youtube.com/channel/UC6kz3lJaZY4wV6olyeZ8nNA"><img src="https://cdn.discordapp.com/attachments/812966246806192128/1350193854057283695/4.png?ex=67d5d984&is=67d48804&hm=6cc8ceaf475441439b6057278bf381c67066eaf82cf73d258b1308949eeba1db&" alt="YouTube"></a>
                            <a href="https://x.com/naanakokona"><img src="https://cdn.discordapp.com/attachments/812966246806192128/1350193853226946593/2.png?ex=67d5d983&is=67d48803&hm=81ad7a1a422f41d87d067d5e5a7125a16201e8cfde1bf625f01573fa0993256c&" alt="Twitter"></a>
                            <a href="https://www.instagram.com/kokonaana._.dayo?igsh=MWwyZjFod2s4dDQyeQ%3D%3D"><img src="https://cdn.discordapp.com/attachments/812966246806192128/1350193853696835624/3.png?ex=67d5d984&is=67d48804&hm=411e0a8a5a76e1787b5d318afb0cba7f9cd6aa62018b79f16d918b40e6e690ea&" alt="Instagram"></a>
                            <a href="https://www.tiktok.com/@kokowanaana"><img src="https://cdn.discordapp.com/attachments/812966246806192128/1350193854413930557/5.png?ex=67d5d984&is=67d48804&hm=971b461097ad8fba1e4a681d65b4b6c56a50420355264313d98f5914b98bb006&" alt="TikTok"></a>
                        </div>
                    </div>
                </div>

                <!-- VTuber 3 -->
                <div class="vtuber-card">
                    <img src="https://cdn.discordapp.com/attachments/812966246806192128/1350209130828140666/2.png?ex=67d6907e&is=67d53efe&hm=7a97e247787f1b455710a25af5b02496ae972645b74fff00ee5074f688fec030&" alt="Aru Masashi" class="vtuber-image">
                    <div class="vtuber-info">
                        <h3 class="vtuber-name">Aru Masashi</h3>
                        <div class="vtuber-role">VTuber / Gamer</div>
                        <p class="vtuber-description">The Coolest Prince from Arcane's Kingdom who defends his kingdom with all his heart and soul.</p>
                        <div class="social-links">
                            <a href="https://www.youtube.com/@aru.masashi"><img src="https://cdn.discordapp.com/attachments/812966246806192128/1350193854057283695/4.png?ex=67d5d984&is=67d48804&hm=6cc8ceaf475441439b6057278bf381c67066eaf82cf73d258b1308949eeba1db&" alt="YouTube"></a>
                            <a href="https://twitter.com/aru_masashi"><img src="https://cdn.discordapp.com/attachments/812966246806192128/1350193853226946593/2.png?ex=67d5d983&is=67d48803&hm=81ad7a1a422f41d87d067d5e5a7125a16201e8cfde1bf625f01573fa0993256c&" alt="Twitter"></a>
                            <a href="https://www.instagram.com/aru.masashi/"><img src="https://cdn.discordapp.com/attachments/812966246806192128/1350193853696835624/3.png?ex=67d5d984&is=67d48804&hm=411e0a8a5a76e1787b5d318afb0cba7f9cd6aa62018b79f16d918b40e6e690ea&" alt="Instagram"></a>
                            <a href="https://www.tiktok.com/@aru.masashii?enable_tiktok_webview=true"><img src="https://cdn.discordapp.com/attachments/812966246806192128/1350193854413930557/5.png?ex=67d5d984&is=67d48804&hm=971b461097ad8fba1e4a681d65b4b6c56a50420355264313d98f5914b98bb006&" alt="TikTok"></a>
                        </div>
                    </div>
                </div>

                <!-- VTuber 4 -->
                <div class="vtuber-card">
                    <img src="https://cdn.discordapp.com/attachments/812966246806192128/1350208740783161426/IMG_20250226_035752_687.webp?ex=67d5e761&is=67d495e1&hm=f233857c6a98851c90d7ad37f82f1ec3b603bd642e2ef1619f13b865fbcc42ab&" alt="Felix Kato" class="vtuber-image">
                    <div class="vtuber-info">
                        <h3 class="vtuber-name">Felix Kato</h3>
                        <div class="vtuber-role">VTuber / Gamer / Digital Artist</div>
                        <p class="vtuber-description">The Ghostly Guardian of the Internet Café.</p>
                        <div class="social-links">
                            <a href="https://youtube.com/@felix_kato?si=OKUX7_dnAsQjA93E"><img src="https://cdn.discordapp.com/attachments/812966246806192128/1350193854057283695/4.png?ex=67d5d984&is=67d48804&hm=6cc8ceaf475441439b6057278bf381c67066eaf82cf73d258b1308949eeba1db&" alt="YouTube"></a>
                            <a href="https://x.com/FelixKato_"><img src="https://cdn.discordapp.com/attachments/812966246806192128/1350193853226946593/2.png?ex=67d5d983&is=67d48803&hm=81ad7a1a422f41d87d067d5e5a7125a16201e8cfde1bf625f01573fa0993256c&" alt="Twitter"></a>
                            <a href="https://www.instagram.com/felix_nyannn"><img src="https://cdn.discordapp.com/attachments/812966246806192128/1350193853696835624/3.png?ex=67d5d984&is=67d48804&hm=411e0a8a5a76e1787b5d318afb0cba7f9cd6aa62018b79f16d918b40e6e690ea&" alt="Instagram"></a>
                        </div>
                    </div>
                </div>

                <!-- VTuber 5 -->
                <div class="vtuber-card">
                    <img src="https://cdn.discordapp.com/attachments/1302256632163729408/1350487008622936145/new.png?ex=67d6ea89&is=67d59909&hm=02013a9bc88f2d9d56a3c1b3c585f1902566ef618ab4d61bbd990143c3045285&" alt="Rizky Kyoya" class="vtuber-image">
                    <div class="vtuber-info">
                        <h3 class="vtuber-name">Rizky Kyoya</h3>
                        <div class="vtuber-role">VTuber / Gamer</div>
                        <p class="vtuber-description">The Reincarnation of Batik.</p>
                        <div class="social-links">
                            <a href="https://www.youtube.com/@RizkyKyoya"><img src="https://cdn.discordapp.com/attachments/812966246806192128/1350193854057283695/4.png?ex=67d5d984&is=67d48804&hm=6cc8ceaf475441439b6057278bf381c67066eaf82cf73d258b1308949eeba1db&" alt="YouTube"></a>
                            <a href="https://x.com/rizky_kyouya"><img src="https://cdn.discordapp.com/attachments/812966246806192128/1350193853226946593/2.png?ex=67d5d983&is=67d48803&hm=81ad7a1a422f41d87d067d5e5a7125a16201e8cfde1bf625f01573fa0993256c&" alt="Twitter"></a>
                            <a href="https://www.instagram.com/rizky_kyoya"><img src="https://cdn.discordapp.com/attachments/812966246806192128/1350193853696835624/3.png?ex=67d5d984&is=67d48804&hm=411e0a8a5a76e1787b5d318afb0cba7f9cd6aa62018b79f16d918b40e6e690ea&" alt="Instagram"></a>
                            <a href="https://www.tiktok.com/@rizky_kyoya"><img src="https://cdn.discordapp.com/attachments/812966246806192128/1350193854413930557/5.png?ex=67d5d984&is=67d48804&hm=971b461097ad8fba1e4a681d65b4b6c56a50420355264313d98f5914b98bb006&" alt="TikTok"></a>
                        </div>
                    </div>
                </div>

                <!-- VTuber 6 -->
                <div class="vtuber-card">
                    <img src="https://cdn.discordapp.com/attachments/812966246806192128/1350208708009000980/Aduh_gantengnyaaa....jpg?ex=67d5e759&is=67d495d9&hm=37e5badd7e88262c0c79f723f05944afd0a938482803ca8f9eb13f26f26188a2&" alt="Coconatsu" class="vtuber-image">
                    <div class="vtuber-info">
                        <h3 class="vtuber-name">Coconatsu</h3>
                        <div class="vtuber-role">VTuber / Gamer / Cooker</div>
                        <p class="vtuber-description">A Cruel Darklord who comes from the Depths of the Abyss.</p>
                        <div class="social-links">
                            <a href="https://www.youtube.com/@KokoNatsuuu"><img src="https://cdn.discordapp.com/attachments/812966246806192128/1350193854057283695/4.png?ex=67d5d984&is=67d48804&hm=6cc8ceaf475441439b6057278bf381c67066eaf82cf73d258b1308949eeba1db&" alt="YouTube"></a>
                            <a href="https://x.com/KokoNatsuuu_"><img src="https://cdn.discordapp.com/attachments/812966246806192128/1350193853226946593/2.png?ex=67d5d983&is=67d48803&hm=81ad7a1a422f41d87d067d5e5a7125a16201e8cfde1bf625f01573fa0993256c&" alt="Twitter"></a>
                            <a href="https://www.instagram.com/kokonatsuuu_"><img src="https://cdn.discordapp.com/attachments/812966246806192128/1350193853696835624/3.png?ex=67d5d984&is=67d48804&hm=411e0a8a5a76e1787b5d318afb0cba7f9cd6aa62018b79f16d918b40e6e690ea&" alt="Instagram"></a>
                            <a href="https://www.tiktok.com/@kokonatsuuu_"><img src="https://cdn.discordapp.com/attachments/812966246806192128/1350193854413930557/5.png?ex=67d5d984&is=67d48804&hm=971b461097ad8fba1e4a681d65b4b6c56a50420355264313d98f5914b98bb006&" alt="TikTok"></a>
                        </div>
                    </div>
                </div>

                <!-- VTuber 7 -->
                <div class="vtuber-card">
                    <img src="https://cdn.discordapp.com/attachments/812966246806192128/1350208458363764888/Ehehemmmnn___art_by___Elysiaa_-__phourw_WEBP.webp?ex=67d5e71e&is=67d4959e&hm=e5906a304f1ec1e1396607d4c469ef91b63f80cdbeb02ac07bd1e722445a786a&" alt="Danny Miraistar" class="vtuber-image">
                    <div class="vtuber-info">
                        <h3 class="vtuber-name">Danny Miraistar</h3>
                        <div class="vtuber-role">VTuber / Gamer</div>
                        <p class="vtuber-description">A High Human who loves discovering and exploring Japanese events on Earth.</p>
                        <div class="social-links">
                            <a href="https://youtube.com/@dannyvtuberid5276?si=OmGDkHLw1OGoz2GE"><img src="https://cdn.discordapp.com/attachments/812966246806192128/1350193854057283695/4.png?ex=67d5d984&is=67d48804&hm=6cc8ceaf475441439b6057278bf381c67066eaf82cf73d258b1308949eeba1db&" alt="YouTube"></a>
                            <a href="https://x.com/DannyVtuberID?t=9HHmk-DezkMoh5E9DONOfw&s=09"><img src="https://cdn.discordapp.com/attachments/812966246806192128/1350193853226946593/2.png?ex=67d5d983&is=67d48803&hm=81ad7a1a422f41d87d067d5e5a7125a16201e8cfde1bf625f01573fa0993256c&" alt="Twitter"></a>
                            <a href="https://www.instagram.com/dannymiraistar"><img src="https://cdn.discordapp.com/attachments/812966246806192128/1350193853696835624/3.png?ex=67d5d984&is=67d48804&hm=411e0a8a5a76e1787b5d318afb0cba7f9cd6aa62018b79f16d918b40e6e690ea&" alt="Instagram"></a>
                            <a href="https://www.tiktok.com/@dannymiraistar?_t=ZS-8ucy1JfHsPw&_r=1"><img src="https://cdn.discordapp.com/attachments/812966246806192128/1350193854413930557/5.png?ex=67d5d984&is=67d48804&hm=971b461097ad8fba1e4a681d65b4b6c56a50420355264313d98f5914b98bb006&" alt="TikTok"></a>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Schedule Section -->
        <section id="schedule" class="schedule">
            <h2 class="schedule-title">Streaming Schedule</h2>
            <p style="text-align: center; margin-bottom: 20px;">Check out when your favorite VTubers are going live!</p>

            <!-- Desktop Schedule -->
            <div class="desktop-schedule">
                <div class="day">
                    <h3>Monday</h3>
                    <p>Ryuga Ranjaya  : -</p>
                    <p>Kokona Naana   : -</p>
                    <p>Aru Masashi    : -</p>
                    <p>Felix Kato     : -</p>
                    <p>Rizky Kyoya    : 14:00</p>
                    <p>Coconatsu      : -</p>
                    <p>Danny Miraistar: -</p>
                </div>
                <div class="day">
                    <h3>Tuesday</h3>
                    <p>Ryuga Ranjaya  : -</p>
                    <p>Kokona Naana   : -</p>
                    <p>Aru Masashi    : -</p>
                    <p>Felix Kato     : -</p>
                    <p>Rizky Kyoya    : 14:00</p>
                    <p>Coconatsu      : -</p>
                    <p>Danny Miraistar: -</p>
                </div>
                <div class="day">
                    <h3>Wednesday</h3>
                    <p>Ryuga Ranjaya  : -</p>
                    <p>Kokona Naana   : -</p>
                    <p>Aru Masashi    : -</p>
                    <p>Felix Kato     : -</p>
                    <p>Rizky Kyoya    : 14:00</p>
                    <p>Coconatsu      : -</p>
                    <p>Danny Miraistar: -</p>
                </div>
                <div class="day">
                    <h3>Thursday</h3>
                    <p>Ryuga Ranjaya  : -</p>
                    <p>Kokona Naana   : -</p>
                    <p>Aru Masashi    : -</p>
                    <p>Felix Kato     : -</p>
                    <p>Rizky Kyoya    : 14:00</p>
                    <p>Coconatsu      : -</p>
                    <p>Danny Miraistar: -</p>
                </div>
                <div class="day">
                    <h3>Friday</h3>
                    <p>Ryuga Ranjaya  : -</p>
                    <p>Kokona Naana   : -</p>
                    <p>Aru Masashi    : -</p>
                    <p>Felix Kato     : 14.00</p>
                    <p>Rizky Kyoya    : 14:00</p>
                    <p>Coconatsu      : -</p>
                    <p>Danny Miraistar: -</p>
                </div>
                <div class="day">
                    <h3>Saturday</h3>
                    <p>Ryuga Ranjaya  : -</p>
                    <p>Kokona Naana   : -</p>
                    <p>Aru Masashi    : -</p>
                    <p>Felix Kato     : -</p>
                    <p>Rizky Kyoya    : Optional</p>
                    <p>Coconatsu      : -</p>
                    <p>Danny Miraistar: -</p>
                </div>
                <div class="day">
                    <h3>Sunday</h3>
                    <p>Ryuga Ranjaya  : -</p>
                    <p>Kokona Naana   : -</p>
                    <p>Aru Masashi    : -</p>
                    <p>Felix Kato     : -</p>
                    <p>Rizky Kyoya    : Optional</p>
                    <p>Coconatsu      : -</p>
                    <p>Danny Miraistar: -</p>
                </div>
            </div>

            <!-- Mobile Schedule -->
            <div class="mobile-schedule">
                <div class="vtuber-schedule" onclick="toggleSchedule(this)">
                    <h3>Rizky Kyoya</h3>
                    <p>Mon-Fri: 14:00, Sat-Sun: Optional</p>
                </div>
                <div class="vtuber-schedule" onclick="toggleSchedule(this)">
                    <h3>Felix Kato</h3>
                    <p>No scheduled streams.</p>
                </div>
                <div class="vtuber-schedule" onclick="toggleSchedule(this)">
                    <h3>Coconatsu</h3>
                    <p>No scheduled streams.</p>
                </div>
                <div class="vtuber-schedule" onclick="toggleSchedule(this)">
                    <h3>Kokona Naana</h3>
                    <p>No scheduled streams.</p>
                </div>
                <div class="vtuber-schedule" onclick="toggleSchedule(this)">
                    <h3>Ryuga Ranjaya</h3>
                    <p>No scheduled streams.</p>
                </div>
                <div class="vtuber-schedule" onclick="toggleSchedule(this)">
                    <h3>Danny Miraistar</h3>
                    <p>No scheduled streams.</p>
                </div>
                <div class="vtuber-schedule" onclick="toggleSchedule(this)">
                    <h3>Aru Masashi</h3>
                    <p>No scheduled streams.</p>
                </div>
            </div>
        </section>
    </main>

    <footer>
        <div class="container">
            <p>&copy; 2025 HARŪNIE VTuber Group. All rights reserved.</p>
        </div>
    </footer>

    <script>
        // JavaScript untuk toggle schedule di mobile
        function toggleSchedule(element) {
            element.classList.toggle("active");
        }
    </script>
</body>
</html>
