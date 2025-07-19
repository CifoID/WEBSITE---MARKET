<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cifo.id - Cinematic Foto Indonesia - Roblox Photography</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700&display=swap');
        @import url('https://fonts.googleapis.com/css2?family=Rubik:wght@400;700&display=swap');

        :root {
            --primary: #FF6B00;
            --secondary: #00A8E8;
            --accent: #FFD166;
            --dark: #2F2F2F;
            --light: #F8F9FA;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Poppins', sans-serif;
            background-color: #121212;
            color: white;
            background-image: url('https://placehold.co/1920x1080/1a1a1a/333333?text=Roblox+Photography+Background&font=roboto');
            background-size: cover;
            background-attachment: fixed;
            background-position: center;
            line-height: 1.6;
            position: relative;
        }

        body::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.85);
            z-index: -1;
        }

        header {
            padding: 1.5rem 2rem;
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            text-align: center;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.3);
            border-bottom: 3px solid var(--accent);
        }

        .logo {
            font-family: 'Rubik', sans-serif;
            font-size: 2.5rem;
            font-weight: 700;
            color: white;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
            letter-spacing: 1px;
        }

        .logo span {
            color: var(--accent);
        }

        .tagline {
            font-size: 1.1rem;
            margin-top: 0.5rem;
            color: rgba(255, 255, 255, 0.9);
        }

        .container {
            max-width: 1200px;
            margin: 2rem auto;
            padding: 0 1.5rem;
        }

        .intro {
            text-align: center;
            margin-bottom: 3rem;
            padding: 2rem;
            background: rgba(18, 18, 18, 0.7);
            border-radius: 10px;
            border-left: 4px solid var(--primary);
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2);
        }

        h1 {
            color: var(--accent);
            margin-bottom: 1rem;
            font-size: 2.2rem;
        }

        h2 {
            color: var(--primary);
            margin: 2rem 0 1rem;
            font-size: 1.8rem;
            position: relative;
            padding-bottom: 0.5rem;
        }

        h2::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 80px;
            height: 3px;
            background: linear-gradient(to right, var(--primary), var(--secondary));
        }

        p {
            margin-bottom: 1rem;
        }

        .highlight {
            color: var(--accent);
            font-weight: 600;
        }

        .pricing-container {
            display: flex;
            justify-content: space-between;
            flex-wrap: wrap;
            gap: 2rem;
            margin-bottom: 3rem;
        }

        .pricing-card {
            background: rgba(18, 18, 18, 0.8);
            border-radius: 10px;
            padding: 2rem;
            flex: 1;
            min-width: 300px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
            border-top: 4px solid var(--secondary);
            transition: transform 0.3s ease;
        }

        .pricing-card:hover {
            transform: translateY(-5px);
        }

        .pricing-card h3 {
            color: var(--primary);
            font-size: 1.5rem;
            margin-bottom: 1.5rem;
            text-align: center;
        }

        .price {
            font-size: 2rem;
            font-weight: 700;
            color: var(--accent);
            text-align: center;
            margin: 1.5rem 0;
        }

        .features {
            list-style: none;
        }

        .features li {
            padding: 0.5rem 0;
            position: relative;
            padding-left: 1.8rem;
        }

        .features li::before {
            content: '✓';
            color: var(--primary);
            position: absolute;
            left: 0;
            font-weight: bold;
        }

        .whatsapp-btn {
            display: inline-block;
            background: #25D366;
            color: white;
            text-decoration: none;
            padding: 1rem 2rem;
            border-radius: 50px;
            font-weight: 600;
            margin-top: 2rem;
            transition: all 0.3s ease;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
            text-align: center;
            font-size: 1.1rem;
            border: none;
            cursor: pointer;
            width: 100%;
        }

        .whatsapp-btn:hover {
            background: #128C7E;
            transform: translateY(-2px);
            box-shadow: 0 6px 15px rgba(0, 0, 0, 0.3);
        }

        .btn-wrapper {
            text-align: center;
            margin: 3rem 0;
        }

        .contact {
            background: rgba(18, 18, 18, 0.8);
            padding: 2rem;
            border-radius: 10px;
            margin-top: 3rem;
            border-left: 4px solid var(--secondary);
        }

        .contact h2 {
            text-align: center;
        }

        .contact-info {
            text-align: center;
            font-size: 1.1rem;
        }

        .email {
            color: var(--accent);
            font-weight: 600;
            text-decoration: none;
        }

        .email:hover {
            text-decoration: underline;
        }

        footer {
            text-align: center;
            padding: 2rem;
            background: rgba(0, 0, 0, 0.5);
            margin-top: 3rem;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
        }

        @media (max-width: 768px) {
            .pricing-container {
                flex-direction: column;
            }
            
            .pricing-card {
                min-width: 100%;
            }
            
            .logo {
                font-size: 2rem;
            }
        }

        /* Animations */
        @keyframes float {
            0% { transform: translateY(0px); }
            50% { transform: translateY(-10px); }
            100% { transform: translateY(0px); }
        }

        .floating {
            animation: float 3s ease-in-out infinite;
        }
    </style>
</head>
<body>
    <header>
        <div class="logo">Cifo<span>.id</span></div>
        <div class="tagline">Cinematic Foto Indonesia - Roblox CDID Photography Specialist</div>
    </header>

    <div class="container">
        <section class="intro">
            <h1>Jasa Fotografi & Cinematic CDID Profesional</h1>
            <p>Memberikan pengalaman fotografi virtual terbaik dengan hasil <span class="highlight">HD berkualitas tinggi</span> untuk avatar, game, dan properti CDID Anda. Kami menawarkan berbagai paket dengan <span class="highlight">harga terjangkau</span> dan hasil yang memuaskan.</p>
            <p>Custom request? Bisa! Cukup beritahu kami apa yang Anda butuhkan.</p>
        </section>

        <h2>Paket Cinematic Roblox</h2>
        <p>Harga mulai dari 10rb tergantung tingkat kesulitan, tidak ada batasan angle kamera, bebas pilih potrait/landscape</p>

        <div class="pricing-container">
            <div class="pricing-card">
                <h3>Paket Basic</h3>
                <div class="price">Rp10.000</div>
                <ul class="features">
                    <li>Durasi 30 detik cinematic</li>
                    <li>maximal klip 7</li>
                    <li>Edit dasar + efek ringan</li>
                    <li>Gaya bebas (portrait/landscape)</li>
                    <li>Pengiriman cepat</li>
                </ul>
            </div>

            <div class="pricing-card">
                <h3>Paket Standard</h3>
                <div class="price">Rp25.000</div>
                <ul class="features">
                    <li>Durasi 1 menit cinematic</li>
                    <li>14</li>
                    <li>Edit profesional + efek cinematic</li>
                    <li>Pilihan resolusi HD/FHD</li>
                    <li>Revisi 1x</li>
                    <li>Pengiriman cepat</li>
                </ul>
            </div>

            <div class="pricing-card">
                <h3>Paket Premium</h3>
                <div class="price">Rp50.000</div>
                <ul class="features">
                    <li>Durasi 2+ menit cinematic</li>
                    <li>bebas klip</li>
                    <li>Edit premium + efek cinematic kompleks</li>
                    <li>Resolusi 4K (jika didukung)</li>
                    <li>Storytelling sequence</li>
                    <li>Revisi 2x</li>
                    <li>Prioritas & pengiriman cepat</li>
                </ul>
            </div>
        </div>

        <h2>Paket Foto Shoot Roblox</h2>
        <p>Mulai dari 3rb/foto hingga maksimal 30rb untuk 25 foto. Bebas pilih angle kamera dengan edit HD</p>

        <div class="pricing-container">
            <div class="pricing-card">
                <h3>Paket Mini</h3>
                <div class="price">Rp3.000/foto</div>
                <ul class="features">
                    <li>Minimal 2 foto</li>
                    <li>bebas angle kamera per foto</li>
                    <li>Edit dasar + color grading</li>
                    <li>Background sederhana</li>
                    <li>Pengiriman dalam 1 hari</li>
                </ul>
            </div>

            <div class="pricing-card">
                <h3>Paket Reguler</h3>
                <div class="price">Rp20.000 (10 foto)</div>
                <ul class="features">
                    <li>10 foto HD</li>
                    <li>bebas angle kamera tak terbatas</li>
                    <li>Edit profesional + efek</li>
                    <li>Background custom</li>
                    <li>Pose request</li>
                    <li>Revisi 1x</li>
                </ul>
            </div>

            <div class="pricing-card">
                <h3>Paket Ultimate</h3>
                <div class="price">Rp35.000 (30 foto)</div>
                <ul class="features">
                    <li>25 foto kualitas premium</li>
                    <li>Angle kamera tak terbatas</li>
                    <li>Editing cinematic profesional</li>
                    <li>Multi-location</li>
                    <li>Story concept</li>
                    <li>Revisi 2x</li>
                    <li>Pengiriman ekspres</li>
                </ul>
            </div>
        </div>

        <div class="btn-wrapper">
            <a href="https://wa.me/6281292211058?text=Halo%20Cifo.id,%20saya%20ingin%20order%20jasa%20foto/cinematic%20Roblox" class="whatsapp-btn">Pesan Sekarang via WhatsApp</a>
        </div>

        <section class="contact">
            <h2>Hubungi Kami</h2>
            <div class="contact-info">
                <p>Email: <a href="mailto:Cifo.idn@gmail.com" class="email">Cifo.idn@gmail.com</a></p>
                <p>WhatsApp: 081292211058</p>
                <p>Media sosial tiktok: CIFO.ID</p>
            </div>
        </section>
    </div>

    <footer>
        <p>&copy; 2025 Cifo.id - Cinematic Foto Indonesia. All Rights Reserved.</p>
    </footer>

    <script>
        // Simple script for smooth scrolling
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });

        // Animation for pricing cards on scroll
        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.style.opacity = 1;
                    entry.target.style.transform = 'translateY(0)';
                }
            });
        }, { threshold: 0.1 });

        document.querySelectorAll('.pricing-card').forEach(card => {
            card.style.opacity = 0;
            card.style.transform = 'translateY(20px)';
            card.style.transition = 'opacity 0.5s ease, transform 0.5s ease';
            observer.observe(card);
        });
    </script>
</body>
</html>
