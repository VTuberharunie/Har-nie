
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HARŪNIE VTuber Group</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f0f2f5;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }
        
        header {
            background: #f9f9f9;
            color: white;
            padding: 15px 0;
            text-align: center;
        }
        
        .logo {
            font-size: 32px;
            font-weight: bold;
        }
        
        nav {
            background-color: #8a5ac9;
            padding: 10px 0;
        }
        
        .menu {
            display: flex;
            justify-content: center;
            list-style-type: none;
            margin: 0;
            padding: 0;
        }
        
        .menu li {
            margin: 0 15px;
        }
        
        .menu a {
            color: white;
            text-decoration: none;
            font-weight: bold;
            font-size: 18px;
        }
        
        .menu a:hover {
            text-decoration: none;
        }
        
        .hero {
            background-color: #9146ff;
            color: white;
            text-align: center;
            padding: 50px 0;
            margin-bottom: 30px;
        }
        
        .hero h1 {
            font-size: 48px;
            margin-bottom: 20px;
        }
        
        .hero p {
            font-size: 20px;
            max-width: 800px;
            margin: 0 auto;
        }
        
        .section-title {
            text-align: center;
            font-size: 36px;
            margin-bottom: 30px;
            color: #6441a5;
        }
        
        .vtubers-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 20px;
        }
        
        .vtuber-card {
            background-color: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s ease;
        }
        
        .vtuber-card:hover {
            transform: translateY(-10px);
        }
        
        .vtuber-image {
            width: 100%;
            height: 250px;
            object-fit: cover;
        }
        
        .vtuber-info {
            padding: 20px;
        }
        
        .vtuber-name {
            font-size: 24px;
            margin-bottom: 10px;
            color: #6441a5;
        }
        
        .vtuber-role {
            font-size: 18px;
            color: #9146ff;
            margin-bottom: 15px;
        }
        
        .vtuber-description {
            color: #333;
            margin-bottom: 15px;
        }
        
        .social-links {
            display: flex;
            gap: 10px;
        }
        
        .social-button {
            background-color: #6441a5;
            color: white;
            border: none;
            padding: 8px 12px;
            border-radius: 5px;
            cursor: pointer;
            text-decoration: none;
            font-size: 14px;
        }
        
        .schedule {
            background-color: white;
            padding: 30px;
            border-radius: 10px;
            margin-top: 40px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }
        
        .schedule-title {
            text-align: center;
            font-size: 28px;
            margin-bottom: 20px;
            color: #6441a5;
        }
        
        footer {
            background-color: #6441a5;
            color: white;
            text-align: center;
            padding: 20px 0;
            margin-top: 40px;
        }
        
        @media (max-width: 800px) {
            .vtubers-grid {
                grid-template-columns: repeat(2, 1fr);
            }
        }
        
        @media (max-width: 500px) {
            .vtubers-grid {
                grid-template-columns: 1fr;
            }
            
            .menu {
                flex-direction: column;
                align-items: center;
            }
            
            .menu li {
                margin: 5px 0;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="center" style="display: flex; justify-content: center; align-items: center;">          
            <img src="https://cdn.discordapp.com/attachments/812966246806192128/1350186993019261088/HARUNIE_1.png?ex=67d5d320&is=67d481a0&hm=88ee16f82aecd510b053a23b30c7a64b8236c4ee3936d7a138f81ed5816c169c&" alt="Harunie Logo" style="height: 200px; margin-right: 100px;">
        </div>
    </header>
    
    <nav>
        <div class="container" style="display: flex; justify-content: space-between; align-items: center;">
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
        <div class="container" style="display: flex; justify-content: space-between; align-items: center;">
            <h1>Welcome to HARŪNIE VTuber Group</h1>
            <p>Discover our amazing virtual talents bringing joy and entertainment to fans worldwide!</p>
        </div>
    </section>
    
    <main class="container">
        <section id="vtubers">
            <h2 class="section-title">Our VTubers</h2>
            
            <div class="vtubers-grid">
                <!-- VTuber 1 -->
                <div class="vtuber-card">
                    <img src="https://cdn.discordapp.com/attachments/812966246806192128/1350208575179587735/IMG_1094.png?ex=67d5e739&is=67d495b9&hm=ef457c0aba708a40f68f8365113122754da8e86a30287d9c8e83c2aee077c57a&" alt="Ryuga Ranjaya" class="vtuber-image">
                    <div class="vtuber-info">
                        <h3 class="vtuber-name">Ryuga Ranjaya</h3>
                        <div class="vtuber-role">VTuber / Gamer</div>
                        <p class="vtuber-description">Ryuga Ranjaya is the Spirit Wolf King tasked with maintaining the balance of the world.</p>
                        <div class="social-links">
                            <a href="https://youtube.com/@ryugaranjaya?si=P5IptDy9svmC4Gyx" class="social-button"><img src="https://cdn.discordapp.com/attachments/812966246806192128/1350193854057283695/4.png?ex=67d5d984&is=67d48804&hm=6cc8ceaf475441439b6057278bf381c67066eaf82cf73d258b1308949eeba1db&" alt="YouTube" style="width: 20px;"></a>
                            <a href="https://twitter.com/RyugaRanjayaa?t=MiGvSFFbUYrJTBBUf4F5FQ&s=09" class="social-button"><img src="https://cdn.discordapp.com/attachments/812966246806192128/1350193853226946593/2.png?ex=67d5d983&is=67d48803&hm=81ad7a1a422f41d87d067d5e5a7125a16201e8cfde1bf625f01573fa0993256c&" alt="Twitter" style="width: 20px;"></a>
                            <a href="https://www.instagram.com/ryugaranjaya" class="social-button"><img src="https://cdn.discordapp.com/attachments/812966246806192128/1350193853696835624/3.png?ex=67d5d984&is=67d48804&hm=411e0a8a5a76e1787b5d318afb0cba7f9cd6aa62018b79f16d918b40e6e690ea&" alt="Instagram" style="width: 20px;"></a>
                            <a href="https://www.tiktok.com/@ryugaranjaya" class="social-button"><img src="https://cdn.discordapp.com/attachments/812966246806192128/1350193854413930557/5.png?ex=67d5d984&is=67d48804&hm=971b461097ad8fba1e4a681d65b4b6c56a50420355264313d98f5914b98bb006&" alt="TikTok" style="width: 20px;"></a>
                        </div>
                    </div>
                </div>
                
                <!-- VTuber 2 -->
                <div class="vtuber-card">
                    <img src="https://cdn.discordapp.com/attachments/812966246806192128/1350208620062576700/Naana_milktea.png?ex=67d5e744&is=67d495c4&hm=b8aa0d6cd765aecb4521b328d0f990a253dd2185df51e32a644a2a14d6d91981&" alt="Nana" class="vtuber-image">
                    <div class="vtuber-info">
                        <h3 class="vtuber-name">Kokona Naana</h3>
                        <div class="vtuber-role">VTuber / Gamer</div>
                        <p class="vtuber-description">An ordinary college student</p>
                        <div class="social-links">
                            <a href="https://www.youtube.com/channel/UC6kz3lJaZY4wV6olyeZ8nNA" class="social-button"><img src="https://cdn.discordapp.com/attachments/812966246806192128/1350193854057283695/4.png?ex=67d5d984&is=67d48804&hm=6cc8ceaf475441439b6057278bf381c67066eaf82cf73d258b1308949eeba1db&" alt="YouTube" style="width: 20px;"></a>
                            <a href="https://x.com/naanakokona" class="social-button"><img src="https://cdn.discordapp.com/attachments/812966246806192128/1350193853226946593/2.png?ex=67d5d983&is=67d48803&hm=81ad7a1a422f41d87d067d5e5a7125a16201e8cfde1bf625f01573fa0993256c&" alt="Twitter" style="width: 20px;"></a>
                            <a href="https://www.instagram.com/kokonaana._.dayo?igsh=MWwyZjFod2s4dDQyeQ%3D%3D" class="social-button"><img src="https://cdn.discordapp.com/attachments/812966246806192128/1350193853696835624/3.png?ex=67d5d984&is=67d48804&hm=411e0a8a5a76e1787b5d318afb0cba7f9cd6aa62018b79f16d918b40e6e690ea&" alt="Instagram" style="width: 20px;"></a>
                            <a href="https://www.tiktok.com/@kokowanaana" class="social-button"><img src="https://cdn.discordapp.com/attachments/812966246806192128/1350193854413930557/5.png?ex=67d5d984&is=67d48804&hm=971b461097ad8fba1e4a681d65b4b6c56a50420355264313d98f5914b98bb006&" alt="TikTok" style="width: 20px;"></a>
                        </div>
                    </div>
                </div>
                
                <!-- VTuber 3 -->
                <div class="vtuber-card">
                    <img src="https://cdn.discordapp.com/attachments/1302256632163729408/1349404778903506984/2.png?ex=67d2faa2&is=67d1a922&hm=d62082d802f1bfeaf1247314d3dc4cc25987c41c4f1c3031ee69b4223f065fa9&" alt="Aru Masashi" class="vtuber-image">
                    <div class="vtuber-info">
                        <h3 class="vtuber-name">Aru Masashi</h3>
                        <div class="vtuber-role">VTuber / Gamer</div>
                        <p class="vtuber-description">The Coolest Prince from Arcane's Kingdom who defends his beyond kingdom with all his heart and soul.</p>
                        <div class="social-links">
                            <a href="https://www.youtube.com/@aru.masashi" class="social-button"><img src="https://cdn.discordapp.com/attachments/812966246806192128/1350193854057283695/4.png?ex=67d5d984&is=67d48804&hm=6cc8ceaf475441439b6057278bf381c67066eaf82cf73d258b1308949eeba1db&" alt="YouTube" style="width: 20px;"></a>
                            <a href="https://twitter.com/aru_masashi" class="social-button"><img src="https://cdn.discordapp.com/attachments/812966246806192128/1350193853226946593/2.png?ex=67d5d983&is=67d48803&hm=81ad7a1a422f41d87d067d5e5a7125a16201e8cfde1bf625f01573fa0993256c&" alt="Twitter" style="width: 20px;"></a>
                            <a href="https://www.instagram.com/aru.masashi/" class="social-button"><img src="https://cdn.discordapp.com/attachments/812966246806192128/1350193853696835624/3.png?ex=67d5d984&is=67d48804&hm=411e0a8a5a76e1787b5d318afb0cba7f9cd6aa62018b79f16d918b40e6e690ea&" alt="Instagram" style="width: 20px;"></a>
                            <a href="https://www.tiktok.com/@aru.masashii?enable_tiktok_webview=true" class="social-button"><img src="https://cdn.discordapp.com/attachments/812966246806192128/1350193854413930557/5.png?ex=67d5d984&is=67d48804&hm=971b461097ad8fba1e4a681d65b4b6c56a50420355264313d98f5914b98bb006&" alt="TikTok" style="width: 20px;"></a>
                        </div>
                    </div>
                </div>
                
                <!-- VTuber 4 -->
                <div class="vtuber-card">
                    <img src="https://cdn.discordapp.com/attachments/812966246806192128/1350208740783161426/IMG_20250226_035752_687.webp?ex=67d5e761&is=67d495e1&hm=f233857c6a98851c90d7ad37f82f1ec3b603bd642e2ef1619f13b865fbcc42ab&" alt="Felix" class="vtuber-image">
                    <div class="vtuber-info">
                        <h3 class="vtuber-name">Felix Kato</h3>
                        <div class="vtuber-role">VTuber/ Gamer / Digital Artist </div>
                        <p class="vtuber-description">The Ghostly Guardian of the Internet Café</p>
                        <div class="social-links">
                            <a href="https://youtube.com/@felix_kato?si=OKUX7_dnAsQjA93E" class="social-button"><img src="https://cdn.discordapp.com/attachments/812966246806192128/1350193854057283695/4.png?ex=67d5d984&is=67d48804&hm=6cc8ceaf475441439b6057278bf381c67066eaf82cf73d258b1308949eeba1db&" alt="YouTube" style="width: 20px;"></a>
                            <a href="https://x.com/FelixKato_" class="social-button" class="social-button"><img src="https://cdn.discordapp.com/attachments/812966246806192128/1350193853226946593/2.png?ex=67d5d983&is=67d48803&hm=81ad7a1a422f41d87d067d5e5a7125a16201e8cfde1bf625f01573fa0993256c&" alt="Twitter" style="width: 20px;"></a>
                            <a href="https://www.instagram.com/felix_nyannn" class="social-button"><img src="https://cdn.discordapp.com/attachments/812966246806192128/1350193853696835624/3.png?ex=67d5d984&is=67d48804&hm=411e0a8a5a76e1787b5d318afb0cba7f9cd6aa62018b79f16d918b40e6e690ea&" alt="Instagram" style="width: 20px;"></a>
                        </div>
                    </div>
                </div>
                
                <!-- VTuber 5 -->
                <div class="vtuber-card">
                    <img src="https://cdn.discordapp.com/attachments/1047949209925591070/1349459778069598269/meaws.png?ex=67d32dda&is=67d1dc5a&hm=8a3a14f7ebdbc2f374d38ca8b28e22ffbbd5d401c31721f6e4938045d8c52c9d&" alt="Rizky" class="vtuber-image">
                    <div class="vtuber-info">
                        <h3 class="vtuber-name">Rizky Kyoya</h3>
                        <div class="vtuber-role">VTuber / Gamer</div>
                        <p class="vtuber-description">The Reincarnation of Batik</p>
                        <div class="social-links">
                            <a href="https://www.youtube.com/@RizkyKyoya" class="social-button"><img src="https://cdn.discordapp.com/attachments/812966246806192128/1350193854057283695/4.png?ex=67d5d984&is=67d48804&hm=6cc8ceaf475441439b6057278bf381c67066eaf82cf73d258b1308949eeba1db&" alt="YouTube" style="width: 20px;"></a>
                            <a href="https://x.com/rizky_kyouya" class="social-button"><img src="https://cdn.discordapp.com/attachments/812966246806192128/1350193853226946593/2.png?ex=67d5d983&is=67d48803&hm=81ad7a1a422f41d87d067d5e5a7125a16201e8cfde1bf625f01573fa0993256c&" alt="Twitter" style="width: 20px;"></a>
                            <a href="https://www.instagram.com/rizky_kyoya" class="social-button"><img src="https://cdn.discordapp.com/attachments/812966246806192128/1350193853696835624/3.png?ex=67d5d984&is=67d48804&hm=411e0a8a5a76e1787b5d318afb0cba7f9cd6aa62018b79f16d918b40e6e690ea&" alt="Instagram" style="width: 20px;"></a>
                            <a href="https://www.tiktok.com/@rizky_kyoya" class="social-button"><img src="https://cdn.discordapp.com/attachments/812966246806192128/1350193854413930557/5.png?ex=67d5d984&is=67d48804&hm=971b461097ad8fba1e4a681d65b4b6c56a50420355264313d98f5914b98bb006&" alt="TikTok" style="width: 20px;"></a>
                        </div>
                    </div>
                </div>
                
                <!-- VTuber 6 -->
                <div class="vtuber-card">
                    <img src="https://cdn.discordapp.com/attachments/812966246806192128/1350208708009000980/Aduh_gantengnyaaa....jpg?ex=67d5e759&is=67d495d9&hm=37e5badd7e88262c0c79f723f05944afd0a938482803ca8f9eb13f26f26188a2&" alt="Coco" class="vtuber-image">
                    <div class="vtuber-info">
                        <h3 class="vtuber-name">Coconatsu</h3>
                        <div class="vtuber-role">VTuber / Gamer / Cooker</div>
                        <p class="vtuber-description">A Cruel Darklord who comes from the Depths of the Abyss</p>
                        <div class="social-links">
                            <a href="https://www.youtube.com/@KokoNatsuuu" class="social-button"><img src="https://cdn.discordapp.com/attachments/812966246806192128/1350193854057283695/4.png?ex=67d5d984&is=67d48804&hm=6cc8ceaf475441439b6057278bf381c67066eaf82cf73d258b1308949eeba1db&" alt="YouTube" style="width: 20px;"></a>
                            <a href="https://x.com/KokoNatsuuu_" class="social-button"><img src="https://cdn.discordapp.com/attachments/812966246806192128/1350193853226946593/2.png?ex=67d5d983&is=67d48803&hm=81ad7a1a422f41d87d067d5e5a7125a16201e8cfde1bf625f01573fa0993256c&" alt="Twitter" style="width: 20px;"></a>
                            <a href="https://www.instagram.com/kokonatsuuu_" class="social-button"><img src="https://cdn.discordapp.com/attachments/812966246806192128/1350193853696835624/3.png?ex=67d5d984&is=67d48804&hm=411e0a8a5a76e1787b5d318afb0cba7f9cd6aa62018b79f16d918b40e6e690ea&" alt="Instagram" style="width: 20px;"></a>
                            <a href="https://www.tiktok.com/@kokonatsuuu_" class="social-button"><img src="https://cdn.discordapp.com/attachments/812966246806192128/1350193854413930557/5.png?ex=67d5d984&is=67d48804&hm=971b461097ad8fba1e4a681d65b4b6c56a50420355264313d98f5914b98bb006&" alt="TikTok" style="width: 20px;"></a>
                        </div>
                    </div>
                </div>
            </div>

             <!-- VTuber 7 -->
             <div class="vtuber-card">
                <img src="https://cdn.discordapp.com/attachments/812966246806192128/1350208458363764888/Ehehemmmnn___art_by___Elysiaa_-__phourw_WEBP.webp?ex=67d5e71e&is=67d4959e&hm=e5906a304f1ec1e1396607d4c469ef91b63f80cdbeb02ac07bd1e722445a786a&" alt="Danny" class="vtuber-image">
                <div class="vtuber-info">
                    <h3 class="vtuber-name">Danny Miraistar </h3>
                    <div class="vtuber-role">VTuber / Gamer</div>
                    <p class="vtuber-description">a High Human who loves discovering and exploring japanese event on Earth</p>
                    <div class="social-links">
                        <a href="https://youtube.com/@dannyvtuberid5276?si=OmGDkHLw1OGoz2GE" class="social-button"><img src="https://cdn.discordapp.com/attachments/812966246806192128/1350193854057283695/4.png?ex=67d5d984&is=67d48804&hm=6cc8ceaf475441439b6057278bf381c67066eaf82cf73d258b1308949eeba1db&" alt="YouTube" style="width: 20px;"></a>
                        <a href="https://x.com/DannyVtuberID?t=9HHmk-DezkMoh5E9DONOfw&s=09" class="social-button"><img src="https://cdn.discordapp.com/attachments/812966246806192128/1350193853226946593/2.png?ex=67d5d983&is=67d48803&hm=81ad7a1a422f41d87d067d5e5a7125a16201e8cfde1bf625f01573fa0993256c&" alt="Twitter" style="width: 20px;"></a>
                        <a href="https://www.instagram.com/dannymiraistar" class="social-button"><img src="https://cdn.discordapp.com/attachments/812966246806192128/1350193853696835624/3.png?ex=67d5d984&is=67d48804&hm=411e0a8a5a76e1787b5d318afb0cba7f9cd6aa62018b79f16d918b40e6e690ea&" alt="Instagram" style="width: 20px;"></a>
                        <a href="https://www.tiktok.com/@dannymiraistar?_t=ZS-8ucy1JfHsPw&_r=1" class="social-button"><img src="https://cdn.discordapp.com/attachments/812966246806192128/1350193854413930557/5.png?ex=67d5d984&is=67d48804&hm=971b461097ad8fba1e4a681d65b4b6c56a50420355264313d98f5914b98bb006&" alt="TikTok" style="width: 20px;"></a>
                    </div>
                </div>
            </div>
        </section>
        
        <section id="schedule" class="schedule">
            <h2 class="schedule-title">Streaming Schedule</h2>
            <p style="text-align: center; margin-bottom: 20px;">Check out when your favorite VTubers are going live!</p>
            
            <div style="overflow-x: auto;">
                <table style="width: 100%; border-collapse: collapse;">
                    <tr style="background-color: #6441a5; color: white;">
                        <th style="padding: 10px; border: 1px solid #ddd;">Nama</th>
                        <th style="padding: 10px; border: 1px solid #ddd;">Monday</th>
                        <th style="padding: 10px; border: 1px solid #ddd;">Tuesday</th>
                        <th style="padding: 10px; border: 1px solid #ddd;">Wednesday</th>
                        <th style="padding: 10px; border: 1px solid #ddd;">Thursday</th>
                        <th style="padding: 10px; border: 1px solid #ddd;">Friday</th>
                        <th style="padding: 10px; border: 1px solid #ddd;">Saturday</th>
                        <th style="padding: 10px; border: 1px solid #ddd;">Sunday</th>
                    </tr>
                    <tr>
                        <td style="padding: 10px; border: 1px solid #ddd; font-weight: bold;">Felix Kato</td>
                        <td style="padding: 10px; border: 1px solid #ddd;">-</td>
                        <td style="padding: 10px; border: 1px solid #ddd;">-</td>
                        <td style="padding: 10px; border: 1px solid #ddd;">-</td>
                        <td style="padding: 10px; border: 1px solid #ddd;">-</td>
                        <td style="padding: 10px; border: 1px solid #ddd;">-</td>
                        <td style="padding: 10px; border: 1px solid #ddd;">-</td>
                        <td style="padding: 10px; border: 1px solid #ddd;">-</td>
                    </tr>
                    <tr style="background-color: #f9f9f9;">
                        <td style="padding: 10px; border: 1px solid #ddd; font-weight: bold;">Coconatsu</td>
                        <td style="padding: 10px; border: 1px solid #ddd;">-</td>
                        <td style="padding: 10px; border: 1px solid #ddd;">-</td>
                        <td style="padding: 10px; border: 1px solid #ddd;">-</td>
                        <td style="padding: 10px; border: 1px solid #ddd;">-</td>
                        <td style="padding: 10px; border: 1px solid #ddd;">-</td>
                        <td style="padding: 10px; border: 1px solid #ddd;">-</td>
                        <td style="padding: 10px; border: 1px solid #ddd;">-</td>
                    </tr>
                    <tr>
                        <td style="padding: 10px; border: 1px solid #ddd; font-weight: bold;">Kokona Naana</td>
                        <td style="padding: 10px; border: 1px solid #ddd;">-</td>
                        <td style="padding: 10px; border: 1px solid #ddd;">-</td>
                        <td style="padding: 10px; border: 1px solid #ddd;">-</td>
                        <td style="padding: 10px; border: 1px solid #ddd;">-</td>
                        <td style="padding: 10px; border: 1px solid #ddd;">-</td>
                        <td style="padding: 10px; border: 1px solid #ddd;">-</td>
                        <td style="padding: 10px; border: 1px solid #ddd;">-</td>
                    </tr>
                    <tr>
                        <td style="padding: 10px; border: 1px solid #ddd; font-weight: bold;">Rizky Kyoya</td>
                        <td style="padding: 10px; border: 1px solid #ddd;">14:00</td>
                        <td style="padding: 10px; border: 1px solid #ddd;">14:00</td>
                        <td style="padding: 10px; border: 1px solid #ddd;">14:00</td>
                        <td style="padding: 10px; border: 1px solid #ddd;">14:00</td>
                        <td style="padding: 10px; border: 1px solid #ddd;">13:00</td>
                        <td style="padding: 10px; border: 1px solid #ddd;">Optional</td>
                        <td style="padding: 10px; border: 1px solid #ddd;">Optional</td>
                    </tr>
                    <tr>
                        <td style="padding: 10px; border: 1px solid #ddd; font-weight: bold;">Ryuga Ranjaya</td>
                        <td style="padding: 10px; border: 1px solid #ddd;">-</td>
                        <td style="padding: 10px; border: 1px solid #ddd;">-</td>
                        <td style="padding: 10px; border: 1px solid #ddd;">-</td>
                        <td style="padding: 10px; border: 1px solid #ddd;">-</td>
                        <td style="padding: 10px; border: 1px solid #ddd;">-</td>
                        <td style="padding: 10px; border: 1px solid #ddd;">-</td>
                        <td style="padding: 10px; border: 1px solid #ddd;">-</td>
                    </tr>
                    <tr>
                        <td style="padding: 10px; border: 1px solid #ddd; font-weight: bold;">Danny Miraistar</td>
                        <td style="padding: 10px; border: 1px solid #ddd;">-</td>
                        <td style="padding: 10px; border: 1px solid #ddd;">-</td>
                        <td style="padding: 10px; border: 1px solid #ddd;">-</td>
                        <td style="padding: 10px; border: 1px solid #ddd;">-</td>
                        <td style="padding: 10px; border: 1px solid #ddd;">-</td>
                        <td style="padding: 10px; border: 1px solid #ddd;">-</td>
                        <td style="padding: 10px; border: 1px solid #ddd;">-</td>
                    </tr>
                    <tr>
                        <td style="padding: 10px; border: 1px solid #ddd; font-weight: bold;">Aru Masashi</td>
                        <td style="padding: 10px; border: 1px solid #ddd;">-</td>
                        <td style="padding: 10px; border: 1px solid #ddd;">-</td>
                        <td style="padding: 10px; border: 1px solid #ddd;">-</td>
                        <td style="padding: 10px; border: 1px solid #ddd;">-</td>
                        <td style="padding: 10px; border: 1px solid #ddd;">-</td>
                        <td style="padding: 10px; border: 1px solid #ddd;">-</td>
                        <td style="padding: 10px; border: 1px solid #ddd;">-</td>
                    </tr>
