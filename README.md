<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HARŪNIE VTuber Group</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        /* General Styles */
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            background: linear-gradient(135deg, #1a1a1a, #2c3e50);
            color: #fff;
            overflow-x: hidden;
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
            position: relative;
            overflow: hidden;
        }

        .logo-container img {
            height: 150px;
            transition: transform 0.5s ease, opacity 0.5s ease;
            animation: float 3s ease-in-out infinite;
        }

        @keyframes float {
            0%, 100% {
                transform: translateY(0);
            }
            50% {
                transform: translateY(-10px);
            }
        }

        .logo-container img:hover {
            transform: scale(1.1);
            opacity: 0.8;
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
            transition: color 0.3s ease, transform 0.3s ease;
        }

        nav ul li a:hover {
            color: #ff6f61;
            transform: translateY(-3px);
        }

        /* Hero Section */
     /* Hero Section */
.hero {
    text-align: center;
    padding: 200px 0; /* Padding untuk desktop */
    background: rgba(0, 0, 0, 0.7) url('https://cdn.discordapp.com/attachments/1272172743571537960/1350848003866624211/Tanpa_judul_Konten_Twitter.png?ex=67d83abd&is=67d6e93d&hm=bc179a1f92dfd913d8b42b8585d73872074c968c610bab8ccbce216b61fe1a72&') no-repeat center center;
    background-size: cover;
    margin-bottom: 40px;
    position: relative;
    overflow: hidden;
    transition: background 0.5s ease;
}

.hero h1 {
    font-size: 5rem; /* Ukuran font untuk desktop */
    margin-bottom: 20px;
    animation: fadeIn 2s ease-in-out;
    opacity: 0.9;
    color: #ffffff;
    text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.7);
}

.hero p {
    font-size: 2rem; /* Ukuran font untuk desktop */
    animation: fadeIn 3s ease-in-out;
    opacity: 0.9;
    color: #fcfbf8;
    text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.7);
}

/* Media Query untuk Mobile */
@media (max-width: 768px) {
    .hero {
        padding: 100px 0; /* Padding lebih kecil untuk mobile */
    }

    .hero h1 {
        font-size: 3rem; /* Ukuran font lebih kecil untuk mobile */
    }

    .hero p {
        font-size: 1.5rem; /* Ukuran font lebih kecil untuk mobile */
    }
}
/* Optional: Add a background overlay */
.hero::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background: rgba(255, 255, 255, 0.13); /* Dark overlay */
    z-index: 1; /* Ensure it is behind the text */
}

@keyframes fadeInBackground {
    from {
        opacity: 0;
    }
    to {
        opacity: 1;
    }
}

.hero {
    animation: fadeInBackground 1s ease-in-out; /* Tambahkan animasi fade in */
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
            position: relative;
            overflow: hidden;
        }

        .vtuber-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.3);
        }

        .vtuber-image {
            max-width: 100%;
            border-radius: 10px;
            margin-bottom: 15px;
            transition: transform 0.3s ease;
        }

        .vtuber-card:hover .vtuber-image {
            transform: scale(1.1);
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

        /* Content Section */
        .content {
            padding: 20px 0;
            background: rgba(0, 0, 0, 0.5);
            margin: 20px 0;
            border-radius: 10px;
            opacity: 0;
            animation: fadeInSlide 1s ease-in-out forwards;
        }

        @keyframes fadeInSlide {
            from {
                opacity: 0;
                transform: translateY(20px) translateX(-20px); /* Mulai dari kiri atas */
            }
            to {
                opacity: 1;
                transform: translateY(0) translateX(0); /* Kembali ke posisi normal */
            }
        }

        /* Grid untuk konten */
       .content-grid {
    display: flex;
    overflow-x: auto; /* Membuat konten bisa di-scroll horizontal */
    white-space: nowrap; /* Mencegah konten berpindah ke baris baru */
    gap: 15px; /* Jarak antar item */
    padding: 10px 0; /* Padding untuk tampilan yang lebih baik */
    scroll-behavior: smooth; /* Scroll yang halus */
}

.vtuber-content {
    flex: 0 0 auto; /* Mencegah item mengubah ukuran */
    min-width: 250px; /* Lebar minimal untuk setiap item */
    background: rgba(255, 255, 255, 0.1); /* Latar belakang untuk konten */
    border-radius: 10px; /* Sudut yang melengkung */
    padding: 15px; /* Padding dalam konten */
    transition: transform 0.3s ease, box-shadow 0.3s ease; /* Efek hover */
}

.vtuber-content:hover {
    transform: scale(1.05); /* Efek zoom saat hover */
    box-shadow: 0 10px 20px rgba(0, 0, 0, 0.3); /* Bayangan saat hover */
}

        /* Animasi Hover dan Gradient Background untuk .vtuber-content */
        .vtuber-content {
            background: linear-gradient(135deg, rgba(255, 255, 255, 0.1), rgba(255, 255, 255, 0.05));
            border-radius: 10px;
            padding: 15px;
            min-width: 250px;
            flex: 0 0 auto;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            position: relative;
            overflow: hidden;
        }

        .vtuber-content::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.1), transparent);
            transition: left 0.5s ease;
        }

        .vtuber-content:hover {
            transform: scale(1.05);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.3);
        }

        .vtuber-content:hover::before {
            left: 100%; /* Efek cahaya bergerak */
        }

        /* Style untuk iframe di dalam .vtuber-content */
        .vtuber-content iframe {
            width: 100%;
            height: 150px;
            border-radius: 8px;
            margin-bottom: 10px;
        }

        /* Style untuk teks di dalam .vtuber-content */
        .vtuber-content h3 {
            font-size: 18px;
            margin: 10px 0;
            color: #fff;
        }

        .vtuber-content p {
            font-size: 14px;
            margin: 0;
            color: rgba(255, 255, 255, 0.8);
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .content-grid {
                flex-direction: column;
                overflow-x: hidden;
            }

            .vtuber-content {
                min-width: 100%;
                transform: none !important;
            }

            .vtuber-content:hover {
                transform: none;
            }
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

        /* Responsive Design */
        @media (max-width: 768px) {
            .vtuber-card, .content-card {
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
            <img src="https://cdn.discordapp.com/attachments/1302256632163729408/1349417752028512257/Simple_Modern_Minimalist_Circle_Design_Studio_Logo_1.png?ex=67d7a3f7&is=67d65277&hm=b6cc236c706e17df5d9955bc11837dbe868f9a2e12f37410f8e89bc60bb9bf81&" alt="HARŪNIE Logo">
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
                    <img src="https://cdn.discordapp.com/attachments/1341331138475720798/1350777200252817478/Picsart_25-03-16_17-25-47-091.jpg?ex=67d7f8cc&is=67d6a74c&hm=51574094ac959ba7bc6caa3fdda04dc4b12a642f8249bc3c810c15f26b2bd604&" alt="Ryuga Ranjaya" class="vtuber-image">
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
                    <img src="https://cdn.discordapp.com/attachments/1341331138475720798/1350773157849726987/1.png?ex=67d7f508&is=67d6a388&hm=dc9ef69465824790df32860b2d7bd2f71f3ed28b90c0d10ac925a4ff200b0792&" alt="Kokona Naana" class="vtuber-image">
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
                    <img src="https://cdn.discordapp.com/attachments/1341331138475720798/1350773770343678052/Desain_tanpa_judul.png?ex=67d7f59b&is=67d6a41b&hm=8c44d55f613000b9f01829857d39523ea821eeac01b9f7bad6be1340773cfa09&" alt="Aru Masashi" class="vtuber-image">
                    <div class="vtuber-info">
                        <h3 class="vtuber-name">Aru Masashi</h3>
                        <div class="vtuber-role">VTuber / Gamer</div>
                        <p class="vtuber-des                        <p class="vtuber-description">The Coolest Prince from Arcane's Kingdom who defends his kingdom with all his heart and soul.</p>
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
                    <img src="https://cdn.discordapp.com/attachments/1341331138475720798/1350773564038451230/IMG_20250226_035752_687_1.png?ex=67d7f569&is=67d6a3e9&hm=887d82e91f2e3b98ada47aaa9ebf772f5a28cd51f6d93373fe01847544cae084&" alt="Felix Kato" class="vtuber-image">
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
                    <img src="https://cdn.discordapp.com/attachments/1341331138475720798/1350773628396109864/Aduh_gantengnyaaa.png?ex=67d7f579&is=67d6a3f9&hm=29f51e8ba8ca00bd0e64710422f99023a7f0e432e3e9a9975ff99f2768d1e3df&" alt="Coconatsu" class="vtuber-image">
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
                    <img src="https://cdn.discordapp.com/attachments/1341331138475720798/1350773415732187196/3.png?ex=67d7f546&is=67d6a3c6&hm=a389b682485f389cc0043a6ed34ee99f0e9a4de201f0aca4e23b5eae6d0917a5&" alt="Danny Miraistar" class="vtuber-image">
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

        <section id="content" class="content">
            <h2 class="section-title">Content</h2>
            <div class="content-grid">
                
                <!-- Konten untuk setiap VTuber -->
                <div class="vtuber-content">
                    <h3>Ryuga Ranjaya</h3>
                    <a href="https://youtu.be/ZFf2RN2_xyg?si=nxxOGzVOK2Yq80eD" target="_blank">
                        <img src="https://img.youtube.com/vi/ZFf2RN2_xyg/hqdefault.jpg" alt="Ryuga Ranjaya Video" style="width: 100%; border-radius: 10px; margin-bottom: 15px;">
                    </a>
                    <p>Check out Ryuga's latest YouTube videos and highlights!</p>
                </div>
                <div class="vtuber-content">
                    <h3>Kokona Naana</h3>
                    <a href="https://www.youtube.com/channel/UC6kz3lJaZY4wV6olyeZ8nNA" target="_blank">
                        <img src="https://img.youtube.com/vi/VIDEO_ID/hqdefault.jpg" alt="Kokona Naana Video" style="width: 100%; border-radius: 10px; margin-bottom: 15px;">
                    </a>
                    <p>Watch Kokona's fun and engaging TikTok clips!</p>
                </div>
                <div class="vtuber-content">
                    <h3>Rizky Kyoya</h3>
                    <a href="https://youtu.be/q-6vbO8qISU" target="_blank">
                        <img src="https://cdn.discordapp.com/attachments/1047949209925591070/1350862141430829126/FINISH_imresizer_1.jpg?ex=67d847e8&is=67d6f668&hm=0aa9f63444ff18a444c8b67cbd6773e794b88ab7e0d3d886987f0b01fbc45dfe&" alt="Rizky Kyoya" style="width: 100%; border-radius: 10px; margin-bottom: 15px;">
                    </a>
                    <p>[ MUSIC COVER ] KING - Kanaria by.Rizky Kyoya</p>
                </div>
                <!-- Tambahkan konten untuk VTuber lainnya dengan cara yang sama -->
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
                    <h3>                    <h3>Friday</h3>
                    <p>Ryuga Ranjaya  : -</p>
                    <p>Kokona Naana   : -</p>
                    <p>Aru Masashi    : -</p>
                    <p>Felix Kato     : -</p>
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

        // Animasi tambahan untuk efek hover pada card
        const vtuberCards = document.querySelectorAll('.vtuber-card');
        vtuberCards.forEach(card => {
            card.addEventListener('mouseenter', () => {
                card.style.transform = 'translateY(-10px)';
                card.style.boxShadow = '0 10px 20px rgba(0, 0, 0, 0.3)';
            });
            card.addEventListener('mouseleave', () => {
                card.style.transform = 'translateY(0)';
                card.style.boxShadow = '0 4px 10px rgba(0, 0, 0, 0.3)';
            });
        });

        // Animasi untuk logo
        const logo = document.querySelector('.logo-container img');
        logo.addEventListener('mouseenter', () => {
            logo.style.transform = 'scale(1.1)';
            logo.style.opacity = '0.8';
        });
        logo.addEventListener('mouseleave', () => {
            logo.style.transform = 'scale(1)';
            logo.style.opacity = '1';
        });
    </script>
</body>
</html>
