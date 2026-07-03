<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Grow Greens Farm Fresh | Sustainable AgriTech Partnership</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary-color: #2e7d32;
            --secondary-color: #4caf50;
            --accent-color: #81c784;
            --dark-text: #212121;
            --light-bg: #f9fbf7;
            --white: #ffffff;
            --github-dark: #24292e;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: var(--light-bg);
            color: var(--dark-text);
            line-height: 1.6;
        }

        /* Navigation */
        header {
            background-color: var(--white);
            box-shadow: 0 2px 10px rgba(0,0,0,0.05);
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        .nav-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            max-width: 1200px;
            margin: 0 auto;
            padding: 1rem 2rem;
        }

        .logo {
            font-size: 1.3rem;
            font-weight: 800;
            color: var(--primary-color);
            text-decoration: none;
            letter-spacing: 0.5px;
        }

        nav {
            display: flex;
            align-items: center;
        }

        nav a {
            color: var(--dark-text);
            text-decoration: none;
            margin-left: 1.5rem;
            font-weight: 500;
            transition: color 0.3s;
        }

        nav a:hover {
            color: var(--secondary-color);
        }

        .btn-github-nav {
            background-color: var(--github-dark);
            color: var(--white) !important;
            padding: 0.5rem 1rem;
            border-radius: 5px;
            display: flex;
            align-items: center;
            gap: 0.5rem;
            font-size: 0.9rem;
            transition: background-color 0.3s, transform 0.2s !important;
        }

        .btn-github-nav:hover {
            background-color: #000000;
            transform: translateY(-1px);
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(rgba(46, 125, 50, 0.85), rgba(27, 94, 32, 0.9)), url('https://images.unsplash.com/photo-1585320806297-9794b3e4eeae?auto=format&fit=crop&w=1600&q=80') center/cover no-repeat;
            color: var(--white);
            padding: 10rem 2rem;
            text-align: center;
        }

        .hero h1 {
            font-size: 3.5rem;
            margin-bottom: 1.5rem;
            font-weight: 800;
            letter-spacing: 1px;
        }

        .hero p {
            font-size: 1.4rem;
            max-width: 800px;
            margin: 0 auto 2.5rem auto;
            opacity: 0.95;
        }

        .hero-buttons {
            display: flex;
            justify-content: center;
            gap: 1rem;
            flex-wrap: wrap;
        }

        .btn {
            background-color: var(--white);
            color: var(--primary-color);
            padding: 0.8rem 2rem;
            border: none;
            border-radius: 5px;
            font-size: 1.1rem;
            font-weight: bold;
            cursor: pointer;
            text-decoration: none;
            transition: transform 0.3s, background-color 0.3s, box-shadow 0.3s;
            display: inline-flex;
            align-items: center;
            gap: 0.5rem;
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
        }

        .btn:hover {
            transform: translateY(-2px);
            background-color: #f0f0f0;
            box-shadow: 0 6px 12px rgba(0,0,0,0.15);
        }

        .btn-secondary {
            background-color: transparent;
            color: var(--white);
            border: 2px solid var(--white);
            box-shadow: none;
        }

        .btn-secondary:hover {
            background-color: rgba(255, 255, 255, 0.1);
            color: var(--white);
            box-shadow: none;
        }

        /* Section Global Settings */
        section {
            padding: 6rem 2rem;
            max-width: 1200px;
            margin: 0 auto;
        }

        .section-title {
            text-align: center;
            font-size: 2.5rem;
            color: var(--primary-color);
            margin-bottom: 3.5rem;
            position: relative;
            font-weight: 700;
        }

        .section-title::after {
            content: '';
            display: block;
            width: 60px;
            height: 4px;
            background-color: var(--secondary-color);
            margin: 12px auto 0 auto;
            border-radius: 2px;
        }

        /* About Section */
        .about-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 3rem;
            align-items: center;
        }

        .card {
            background: var(--white);
            padding: 2.5rem;
            border-radius: 12px;
            box-shadow: 0 10px 20px rgba(0,0,0,0.03);
            border-top: 4px solid var(--secondary-color);
            transition: transform 0.3s;
        }

        .card:hover {
            transform: translateY(-5px);
        }

        .card h3 {
            margin-bottom: 1rem;
            color: var(--primary-color);
            display: flex;
            align-items: center;
            gap: 0.75rem;
        }

        /* Problem & Solution Grid */
        .grid-3 {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2.5rem;
        }

        /* Value Propositions */
        .vp-list {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 1.5rem;
        }

        .vp-item {
            background: var(--white);
            padding: 1.5rem;
            border-left: 4px solid var(--primary-color);
            border-radius: 0 12px 12px 0;
            box-shadow: 0 4px 6px rgba(0,0,0,0.02);
            font-weight: 500;
            display: flex;
            align-items: center;
            gap: 0.75rem;
        }

        .vp-item i {
            color: var(--secondary-color);
        }

        /* Team Section */
        .team-grid {
            display: flex;
            justify-content: center;
            gap: 4rem;
            flex-wrap: wrap;
        }

        .team-member {
            background: var(--white);
            padding: 3rem 2.5rem;
            border-radius: 12px;
            text-align: center;
            box-shadow: 0 10px 20px rgba(0,0,0,0.03);
            width: 340px;
            transition: transform 0.3s;
        }

        .team-member:hover {
            transform: translateY(-5px);
        }

        .team-profile-icon {
            font-size: 4rem;
            color: var(--accent-color);
            margin-bottom: 1.5rem;
        }

        .team-member h3 {
            color: var(--primary-color);
            margin-bottom: 0.25rem;
            font-size: 1.4rem;
        }

        .team-member .role {
            font-weight: 700;
            color: var(--secondary-color);
            margin-bottom: 1.5rem;
            font-size: 0.95rem;
            text-transform: uppercase;
            letter-spacing: 0.5px;
        }

        /* Footer */
        footer {
            background-color: #1b5e20;
            color: var(--white);
            text-align: center;
            padding: 4rem 2rem;
            margin-top: 5rem;
        }

        footer .footer-gh-link {
            color: var(--white);
            font-size: 1.5rem;
            margin-top: 1rem;
            display: inline-block;
            transition: opacity 0.3s;
        }

        footer .footer-gh-link:hover {
            opacity: 0.8;
        }

        /* Responsive adjustments */
        @media (max-width: 768px) {
            .about-grid { grid-template-columns: 1fr; gap: 2rem; }
            .hero h1 { font-size: 2.5rem; }
            .hero p { font-size: 1.1rem; }
            .nav-container { flex-direction: column; gap: 1.5rem; text-align: center; }
            nav { flex-wrap: wrap; justify-content: center; gap: 1rem; }
            nav a { margin: 0 0.5rem; }
            .btn-github-nav { margin-left: 0; margin-top: 0.5rem; }
            section { padding: 4rem 1.5rem; }
        }
    </style>
</head>
<body>

    <header>
        <div class="nav-container">
            <a href="#" class="logo">GROW GREENS FARM FRESH</a>
            <nav>
                <a href="#about">About Us</a>
                <a href="#challenges">Challenges</a>
                <a href="#solution">Our Solution</a>
                <a href="#team">Team</a>
                <a href="https://github.com" target="_blank" class="btn-github-nav">
                    <i class="fab fa-github"></i> GitHub
                </a>
            </nav>
        </div>
    </header>

    <section class="hero" style="max-width:100%; width:100%;">
        <h1>GROW GREENS FARM FRESH</h1>
        <p>An innovative Agriculture Partnership Model driving climate-resilient, technology-driven cultivation across India.</p>
        <div class="hero-buttons">
            <a href="#about" class="btn"><i class="fas fa-info-circle"></i> Learn More</a>
            <a href="https://github.com" target="_blank" class="btn btn-secondary"><i class="fab fa-github"></i> View Repository</a>
        </div>
    </section>

    <section id="about">
        <h2 class="section-title">Who is Grow Greens Farm Fresh</h2>
        <div class="about-grid">
            <div>
                <p style="font-size: 1.2rem; margin-bottom: 1.5rem; color: var(--primary-color); font-weight: 600;">Empowering farmers via protected cultivation technology.</p>
                <p style="margin-bottom: 1rem;"><strong>Grow Greens Farm Fresh</strong> is an AgriTech enterprise that collaborates actively with farmers to grow high-quality vegetables using precision polyhouse environments.</p>
                <p>We mitigate climate-related risks, improve crop quality, optimize structural yields, and unlock premium market prices through standard technical frameworks and direct market distribution linkages.</p>
            </div>
            <div style="display: grid; gap: 1.5rem;">
                <div class="card">
                    <h3><i class="fas fa-bullseye"></i> Our Mission</h3>
                    <p>To empower farmers with climate-resilient protected cultivation solutions and maximize their revenue metrics through smart, tech-driven agriculture ecosystems.</p>
                </div>
                <div class="card">
                    <h3><i class="fas fa-eye"></i> Our Vision</h3>
                    <p>To become a leading benchmark AgriTech platform enabling sustainable, profitable, and high-yielding vegetable production across agricultural hubs.</p>
                </div>
            </div>
        </div>
    </section>

    <section id="challenges" style="background-color: #f1f8e9; max-width:100%; width:100%;">
        <div style="max-width: 1200px; margin: 0 auto; padding: 0 2rem;">
            <h2 class="section-title">The Market Challenge</h2>
            <div class="grid-3">
                <div class="card">
                    <h3><i class="fas fa-cloud-sun-rain" style="color:#e65100;"></i> Unpredictable Climate</h3>
                    <p>Traditional open-field farming leaves growers vulnerable to volatile weather shifts, sudden temperature spikes, and irregular monsoon distributions.</p>
                </div>
                <div class="card">
                    <h3><i class="fas fa-chart-line-down" style="color:#c62828;"></i> Crop & Income Losses</h3>
                    <p>Uncontrolled pest environments and shifting market demand produce severe financial losses, leading to low crop yields and unpredictable yearly income.</p>
                </div>
                <div class="card">
                    <h3><i class="fas fa-shield-alt" style="color:#1565c0;"></i> High Barriers to Entry</h3>
                    <p>Small-to-medium farming operators struggle to deploy automated protected cultivation infrastructure independently due to high entry overheads and missing tech workflows.</p>
                </div>
            </div>
        </div>
    </section>

    <section id="solution">
        <h2 class="section-title">The Technology & Solution</h2>
        <p style="text-align: center; max-width: 800px; margin: 0 auto 3.5rem auto; font-size: 1.1rem; color: #555;">
            We deliver modular, production-ready frameworks for sustainable cultivation, blending scientific infrastructure design with data-backed farming practices.
        </p>
        
        <div class="grid-3" style="margin-bottom: 4rem;">
            <div class="card">
                <h3>Advanced Infrastructure</h3>
                <p>Deploying automated microclimate control parameters, precision automated fertigation networks, and continuous data monitoring metrics.</p>
            </div>
            <div class="card">
                <h3>Innovative Growth Methods</h3>
                <p>Integrating modern agritech discoveries, including specialized acoustic frequency plant stimulation configurations to maximize crop response and growth speeds.</p>
            </div>
            <div class="card">
                <h3>End-to-End Support</h3>
                <p>Providing rigorous structural mapping, clean data handoffs, continuous engineering inspection parameters, and premium buyer pipelines.</p>
            </div>
        </div>

        <h3 style="margin-bottom: 2rem; text-align: center; color: var(--primary-color); font-size: 1.75rem;">Customer Value Proposition</h3>
        <div class="vp-list">
            <div class="vp-item"><i class="fas fa-check-circle"></i> absolute protection against climate-linked damage</div>
            <div class="vp-item"><i class="fas fa-check-circle"></i> Predictable volume scaling and product consistency</div>
            <div class="vp-item"><i class="fas fa-check-circle"></i> Sustainable revenue structures for partnering growers</div>
            <div class="vp-item"><i class="fas fa-check-circle"></i> Maximized output compared to open conventional fields</div>
            <div class="vp-item"><i class="fas fa-check-circle"></i> Live, ongoing technical asset advisory loops</div>
            <div class="vp-item"><i class="fas fa-check-circle"></i> Direct interfaces to organized distribution networks</div>
        </div>
        
        <p style="margin-top: 4rem; text-align: center; font-style: italic; color: #555; background: #fff; padding: 1.5rem; border-radius: 8px; box-shadow: 0 4px 10px rgba(0,0,0,0.02);">
            <i class="fas fa-rocket" style="color: var(--secondary-color); margin-right: 0.5rem;"></i> Our model is open-sourced, scalable, and fully optimized for immediate distribution architectures across high-value varieties like cucumbers, capsicums, and cherry tomatoes.
        </p>
    </section>

    <section id="landscape" style="background-color: #f1f8e9; max-width:100%; width:100%;">
        <div style="max-width: 1200px; margin: 0 auto; padding: 0 2rem;">
            <h2 class="section-title">Competitive Advantage & Business Model</h2>
            <div class="about-grid">
                <div class="card">
                    <h3>Why Choose Grow Greens?</h3>
                    <ul style="padding-left: 1.25rem; margin-top: 0.5rem; display: grid; gap: 0.5rem;">
                        <li>Decentralized, risk-mitigating collaborative partnership design.</li>
                        <li>Seamless data workflows from implementation directly to final wholesale delivery.</li>
                        <li>High-precision yield optimization mapping algorithms.</li>
                        <li>Replicable open code blueprints for swift geographical cloning.</li>
                    </ul>
                </div>
                <div class="card">
                    <h3>Target Customers & Revenue</h3>
                    <p><strong>Target Landscape:</strong> Progressive modern farmers, Agribusiness enterprises, ecosystem investors, and local Farmer Producer Organizations (FPOs).</p>
                    <p style="margin-top: 0.75rem;"><strong>Revenue Vectors:</strong> Programmatic yield processing, infrastructure integration partnerships, and high-margin product exports.</p>
                </div>
            </div>
        </div>
    </section>

    <section id="team">
        <h2 class="section-title">Our Team</h2>
        <div class="team-grid">
            <div class="team-member">
                <div class="team-profile-icon"><i class="fas fa-user-tie"></i></div>
                <h3>Siddharth Boricha</h3>
                <div class="role">Founder & CEO</div>
                <p style="font-size: 0.95rem; color: #555;">B.Voc Graduate, currently completing an MBA at Parul University. Focuses on overall ecosystem growth, strategic partnership networking, and core business architecture development.</p>
            </div>
            <div class="team-member">
                <div class="team-profile-icon"><i class="fas fa-seedling"></i></div>
                <h3>Yash Boricha</h3>
                <div class="role">Agriculture Operations Manager</div>
                <p style="font-size: 0.95rem; color: #555;">M.Sc in Biotechnology from Atmiya University. Orchestrates botanical optimization models, infrastructure logic metrics, and crop health algorithms.</p>
            </div>
        </div>
    </section>

    <footer>
        <p>&copy; 2026 Grow Greens Farm Fresh. Enabling Sustainable, Profitable, and High-Quality Agriculture across India.</p>
        <a href="https://github.com" target="_blank" class="footer-gh-link"><i class="fab fa-github"></i></a>
    </footer>

</body>
</html>
