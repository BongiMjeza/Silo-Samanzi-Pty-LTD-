<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Business Website</title>
    <style>
        /* --- GENERAL STYLES --- */
        :root {
            --primary-color: #2c3e50; /* Dark Blue */
            --accent-color: #3498db;  /* Bright Blue */
            --light-bg: #f4f4f4;
            --text-color: #333;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            margin: 0;
            padding: 0;
            line-height: 1.6;
            color: var(--text-color);
        }

        /* --- HEADER & LOGO --- */
        header {
            background: #fff;
            padding: 1rem 5%;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
            display: flex;
            justify-content: space-between;
            align-items: center;
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        .logo {
            font-size: 1.5rem;
            font-weight: bold;
            color: var(--primary-color);
            display: flex;
            align-items: center;
        }

        /* If using an actual image logo, use this class */
        .logo img {
            height: 50px; /* Adjust height as needed */
            margin-right: 10px;
        }

        nav a {
            text-decoration: none;
            color: var(--text-color);
            margin-left: 20px;
            font-weight: 500;
        }

        nav a:hover {
            color: var(--accent-color);
        }

        /* --- HERO SECTION --- */
        .hero {
            background: linear-gradient(rgba(44, 62, 80, 0.8), rgba(44, 62, 80, 0.8)), url('https://source.unsplash.com/random/1600x900/?business,office');
            background-size: cover;
            background-position: center;
            color: white;
            padding: 100px 20px;
            text-align: center;
        }

        .hero h1 {
            font-size: 3rem;
            margin-bottom: 10px;
        }

        .btn {
            display: inline-block;
            background: var(--accent-color);
            color: white;
            padding: 10px 30px;
            border-radius: 5px;
            text-decoration: none;
            margin-top: 20px;
            font-weight: bold;
        }

        .btn:hover {
            background: #2980b9;
        }

        /* --- DETAILS SECTION --- */
        .container {
            padding: 60px 5%;
            max-width: 1200px;
            margin: auto;
        }

        .section-title {
            text-align: center;
            margin-bottom: 40px;
            color: var(--primary-color);
        }

        /* --- BUSINESS TYPES (Grid Layout) --- */
        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
        }

        .service-card {
            background: #fff;
            border: 1px solid #ddd;
            padding: 30px;
            border-radius: 8px;
            text-align: center;
            transition: transform 0.3s ease;
        }

        .service-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }

        .service-card h3 {
            color: var(--primary-color);
        }

        /* --- FOOTER --- */
        footer {
            background: var(--primary-color);
            color: white;
            text-align: center;
            padding: 40px 20px;
            margin-top: auto;
        }

        footer p {
            margin: 5px 0;
        }

        /* Mobile Responsive */
        @media (max-width: 768px) {
            .hero h1 { font-size: 2rem; }
            header { flex-direction: column; }
            nav { margin-top: 15px; }
        }
    </style>
</head>
<body>

    <header>
        <div class="logo">
            YOUR LOGO
        </div>
        <nav>
            <a href="#about">About</a>
            <a href="#services">Services</a>
            <a href="#contact">Contact</a>
        </nav>
    </header>

    <section class="hero">
        <h1>Your Business Name Here</h1>
        <p>Providing excellence and quality service to our customers.</p>
        <a href="#contact" class="btn">Get in Touch</a>
    </section>

    <section id="about" class="container">
        <h2 class="section-title">Who We Are</h2>
        <p style="text-align: center; max-width: 800px; margin: 0 auto;">
            [Insert a brief description of your business here. Explain your mission, 
            how long you have been in business, and what makes you unique.]
        </p>
    </section>

    <section id="services" class="container" style="background-color: var(--light-bg);">
        <h2 class="section-title">Our Business Offerings</h2>
        
        <div class="services-grid">
            <div class="service-card">
                <h3>Service Type A</h3>
                <p>Description of your first business activity or product line.</p>
            </div>

            <div class="service-card">
                <h3>Service Type B</h3>
                <p>Description of your second business activity or product line.</p>
            </div>

            <div class="service-card">
                <h3>Service Type C</h3>
                <p>Description of your third business activity or product line.</p>
            </div>
        </div>
    </section>

    <footer id="contact">
        <h2>Contact Us</h2>
        <p><strong>Address:</strong> 123 Business Road, City, Country</p>
        <p><strong>Phone:</strong> (555) 123-4567</p>
        <p><strong>Email:</strong> info@yourbusiness.com</p>
        <br>
        <p>&copy; 2024 Your Business Name. All Rights Reserved.</p>
    </footer>

</body>
</html>
