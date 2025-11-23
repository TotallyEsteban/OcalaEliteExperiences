<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ocala Elite Experiences | Premium Events at World Equestrian Center</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;500;600;700;800;900&family=Inter:wght@300;400;500;600;700&display=swap');
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            background: #0a0a0a;
            color: #ffffff;
            font-family: 'Inter', sans-serif;
            line-height: 1.6;
        }
        
        h1, h2, h3 {
            font-family: 'Playfair Display', serif;
            letter-spacing: -0.5px;
        }
        
        .gradient-gold {
            background: linear-gradient(135deg, #d4af37 0%, #f4e4c1 50%, #d4af37 100%);
        }
        
        .gradient-text {
            background: linear-gradient(135deg, #d4af37 0%, #f4e4c1 50%, #d4af37 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }
        
        .container {
            max-width: 1280px;
            margin: 0 auto;
            padding: 0 24px;
        }
        
        /* Navigation */
        nav {
            position: fixed;
            top: 0;
            width: 100%;
            background: rgba(10, 10, 10, 0.98);
            backdrop-filter: blur(20px);
            border-bottom: 1px solid rgba(212, 175, 55, 0.15);
            z-index: 1000;
            padding: 24px 0;
        }
        
        nav .container {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .logo {
            display: flex;
            align-items: center;
            gap: 16px;
        }
        
        .logo-text {
            font-family: 'Playfair Display', serif;
            font-weight: 700;
            font-size: 1.5rem;
            letter-spacing: 1px;
        }
        
        .nav-links {
            display: flex;
            gap: 48px;
            align-items: center;
        }
        
        .nav-links a {
            text-decoration: none;
            color: rgba(255, 255, 255, 0.85);
            transition: color 0.3s;
            font-weight: 500;
            letter-spacing: 0.5px;
        }
        
        .nav-links a:hover {
            color: #d4af37;
        }
        
        .btn {
            padding: 14px 32px;
            border-radius: 4px;
            font-weight: 600;
            text-decoration: none;
            display: inline-block;
            transition: all 0.3s;
            border: none;
            cursor: pointer;
            letter-spacing: 0.5px;
        }
        
        .btn-primary {
            color: #0a0a0a;
            box-shadow: 0 4px 14px rgba(212, 175, 55, 0.4);
        }
        
        .btn-primary:hover {
            transform: translateY(-2px);
            box-shadow: 0 6px 20px rgba(212, 175, 55, 0.6);
        }
        
        .btn-secondary {
            border: 2px solid #d4af37;
            color: #d4af37;
            background: transparent;
        }
        
        .btn-secondary:hover {
            background: rgba(212, 175, 55, 0.1);
        }
        
        /* Hero */
        .hero {
            padding: 180px 24px 120px;
            background: linear-gradient(135deg, #0a0a0a 0%, #1a1510 100%);
            position: relative;
            overflow: hidden;
        }
        
        .hero::before {
            content: '';
            position: absolute;
            top: 0;
            right: 0;
            width: 60%;
            height: 100%;
            background: radial-gradient(circle at top right, rgba(212, 175, 55, 0.08) 0%, transparent 70%);
        }
        
        .hero-content {
            position: relative;
            z-index: 1;
            max-width: 900px;
        }
        
        .badge {
            display: inline-block;
            padding: 10px 20px;
            background: rgba(212, 175, 55, 0.1);
            border: 1px solid rgba(212, 175, 55, 0.3);
            border-radius: 4px;
            color: #d4af37;
            font-weight: 600;
            font-size: 12px;
            margin-bottom: 32px;
            letter-spacing: 2px;
            text-transform: uppercase;
        }
        
        h1 {
            font-size: 5rem;
            font-weight: 800;
            line-height: 1.1;
            margin-bottom: 32px;
            letter-spacing: -2px;
        }
        
        h2 {
            font-size: 3.5rem;
            font-weight: 700;
            margin-bottom: 24px;
            letter-spacing: -1px;
        }
        
        h3 {
            font-size: 2rem;
            font-weight: 600;
            margin-bottom: 16px;
        }
        
        .hero-subtitle {
            font-size: 1.4rem;
            color: rgba(255, 255, 255, 0.75);
            margin-bottom: 48px;
            line-height: 1.8;
            font-weight: 300;
        }
        
        .btn-group {
            display: flex;
            gap: 20px;
            margin-bottom: 56px;
        }
        
        .luxury-badges {
            display: flex;
            gap: 48px;
            align-items: center;
            padding-top: 40px;
            border-top: 1px solid rgba(212, 175, 55, 0.2);
        }
        
        .luxury-item {
            display: flex;
            align-items: center;
            gap: 12px;
            color: rgba(255, 255, 255, 0.6);
            font-size: 13px;
            font-weight: 500;
            letter-spacing: 1px;
            text-transform: uppercase;
        }
        
        /* Stats */
        .stats-section {
            background: #0f0f0f;
            padding: 100px 24px;
            border-top: 1px solid rgba(212, 175, 55, 0.1);
            border-bottom: 1px solid rgba(212, 175, 55, 0.1);
        }
        
        .stats-grid {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 64px;
            text-align: center;
        }
        
        .stat-value {
            font-family: 'Playfair Display', serif;
            font-size: 4.5rem;
            font-weight: 800;
            margin-bottom: 12px;
            letter-spacing: -2px;
        }
        
        .stat-label {
            color: rgba(255, 255, 255, 0.5);
            font-size: 13px;
            font-weight: 500;
            text-transform: uppercase;
            letter-spacing: 2px;
        }
        
        /* Services */
        .services {
            padding: 120px 24px;
        }
        
        .section-header {
            text-align: center;
            max-width: 800px;
            margin: 0 auto 80px;
        }
        
        .section-subtitle {
            font-size: 1.2rem;
            color: rgba(255, 255, 255, 0.6);
            margin-top: 20px;
            font-weight: 300;
        }
        
        .services-grid {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 40px;
            margin-top: 80px;
        }
        
        .service-card {
            background: linear-gradient(135deg, rgba(212, 175, 55, 0.03) 0%, rgba(15, 15, 15, 0.8) 100%);
            padding: 64px;
            border-radius: 4px;
            border: 1px solid rgba(212, 175, 55, 0.15);
            transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
            position: relative;
            overflow: hidden;
        }
        
        .service-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 2px;
            background: linear-gradient(90deg, transparent 0%, #d4af37 50%, transparent 100%);
            transform: scaleX(0);
            transition: transform 0.4s;
        }
        
        .service-card:hover {
            transform: translateY(-12px);
            border-color: rgba(212, 175, 55, 0.4);
            box-shadow: 0 24px 48px rgba(0, 0, 0, 0.4);
        }
        
        .service-card:hover::before {
            transform: scaleX(1);
        }
        
        .service-number {
            font-family: 'Playfair Display', serif;
            font-size: 5rem;
            font-weight: 200;
            color: rgba(212, 175, 55, 0.15);
            margin-bottom: -20px;
        }
        
        .service-pricing {
            font-family: 'Playfair Display', serif;
            font-size: 2.5rem;
            font-weight: 600;
            margin: 24px 0 16px;
        }
        
        .service-features {
            list-style: none;
            margin: 24px 0;
        }
        
        .service-features li {
            display: flex;
            align-items: flex-start;
            gap: 12px;
            margin-bottom: 16px;
            color: rgba(255, 255, 255, 0.7);
            font-size: 15px;
        }
        
        .check {
            color: #d4af37;
            font-size: 18px;
            flex-shrink: 0;
            margin-top: 2px;
        }
        
        /* Testimonials */
        .testimonials {
            padding: 120px 24px;
            background: #0f0f0f;
        }
        
        .testimonial-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 40px;
            margin-top: 80px;
        }
        
        .testimonial-card {
            background: linear-gradient(135deg, rgba(212, 175, 55, 0.03) 0%, rgba(15, 15, 15, 0.6) 100%);
            padding: 48px;
            border-radius: 4px;
            border: 1px solid rgba(212, 175, 55, 0.15);
        }
        
        .quote {
            color: #d4af37;
            font-size: 3rem;
            line-height: 1;
            margin-bottom: 20px;
            font-family: 'Playfair Display', serif;
        }
        
        .testimonial-text {
            font-size: 1.1rem;
            line-height: 1.8;
            color: rgba(255, 255, 255, 0.8);
            margin-bottom: 24px;
            font-style: italic;
        }
        
        /* CTA */
        .cta-section {
            padding: 120px 24px;
            background: linear-gradient(135deg, #1a1510 0%, #0a0a0a 100%);
            position: relative;
        }
        
        .cta-content {
            text-align: center;
            max-width: 800px;
            margin: 0 auto;
        }
        
        /* Footer */
        footer {
            background: #0a0a0a;
            padding: 80px 24px 40px;
            border-top: 1px solid rgba(212, 175, 55, 0.1);
        }
        
        .footer-grid {
            display: grid;
            grid-template-columns: 2fr 1fr 1fr 1fr;
            gap: 64px;
            margin-bottom: 64px;
        }
        
        .footer-links {
            list-style: none;
        }
        
        .footer-links li {
            margin-bottom: 16px;
        }
        
        .footer-links a {
            color: rgba(255, 255, 255, 0.5);
            text-decoration: none;
            transition: color 0.3s;
            font-size: 14px;
        }
        
        .footer-links a:hover {
            color: #d4af37;
        }
        
        .footer-bottom {
            padding-top: 40px;
            border-top: 1px solid rgba(212, 175, 55, 0.1);
            text-align: center;
            color: rgba(255, 255, 255, 0.4);
            font-size: 13px;
        }
        
        /* Responsive */
        @media (max-width: 768px) {
            h1 {
                font-size: 3rem;
            }
            
            h2 {
                font-size: 2.5rem;
            }
            
            .nav-links {
                display: none;
            }
            
            .stats-grid,
            .services-grid,
            .testimonial-grid,
            .footer-grid {
                grid-template-columns: 1fr;
            }
            
            .btn-group {
                flex-direction: column;
            }
            
            .luxury-badges {
                flex-wrap: wrap;
            }
        }
    </style>
</head>
<body>
    <!-- Navigation -->
    <nav>
        <div class="container">
            <div class="logo">
                <div class="logo-text gradient-text">Ocala Elite Experiences</div>
            </div>
            <div class="nav-links">
                <a href="#services">Services</a>
                <a href="#testimonials">Testimonials</a>
                <a href="#contact">Contact</a>
                <a href="#contact" class="btn btn-primary gradient-gold">Book Experience</a>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section class="hero">
        <div class="container">
            <div class="hero-content">
                <div class="badge">World Equestrian Center Exclusive</div>
                <h1>
                    Where Excellence<br>
                    <span class="gradient-text">Meets Elegance</span>
                </h1>
                <p class="hero-subtitle">
                    Premium event production and hospitality at the world's premier equestrian venue. 
                    Fortune 500 corporate events, exclusive VIP memberships, and elite rider brand management powered by IATSE Local 631.
                </p>
                <div class="btn-group">
                    <a href="#contact" class="btn btn-primary gradient-gold">Schedule Consultation</a>
                    <a href="#services" class="btn btn-secondary">Explore Services</a>
                </div>
                <div class="luxury-badges">
                    <div class="luxury-item">
                        <span style="color: #d4af37;">◆</span>
                        <span>IATSE Union Crews</span>
                    </div>
                    <div class="luxury-item">
                        <span style="color: #d4af37;">◆</span>
                        <span>WEC Exclusive Partner</span>
                    </div>
                    <div class="luxury-item">
                        <span style="color: #d4af37;">◆</span>
                        <span>Since 2024</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Stats Bar -->
    <section class="stats-section">
        <div class="container">
            <div class="stats-grid">
                <div>
                    <div class="stat-value gradient-text">$22M</div>
                    <div class="stat-label">Annual Events</div>
                </div>
                <div>
                    <div class="stat-value gradient-text">125</div>
                    <div class="stat-label">VIP Members</div>
                </div>
                <div>
                    <div class="stat-value gradient-text">55</div>
                    <div class="stat-label">Corporate Events</div>
                </div>
                <div>
                    <div class="stat-value gradient-text">100%</div>
                    <div class="stat-label">Client Satisfaction</div>
                </div>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section id="services" class="services">
        <div class="container">
            <div class="section-header">
                <h2>Four Signature Services</h2>
                <p class="section-subtitle">
                    Curated experiences for Fortune 500 companies, ultra-high-net-worth individuals, and elite equestrian athletes
                </p>
            </div>

            <div class="services-grid">
                <!-- Corporate Events -->
                <div class="service-card">
                    <div class="service-number">01</div>
                    <h3>Corporate Event Production</h3>
                    <p style="color: rgba(255,255,255,0.6); margin: 20px 0 32px; font-size: 15px;">
                        Full-service event production for Fortune 500 corporate hospitality at World Equestrian Center
                    </p>
                    <ul class="service-features">
                        <li>
                            <span class="check">✓</span>
                            <span>VIP suites and private boxes</span>
                        </li>
                        <li>
                            <span class="check">✓</span>
                            <span>Celebrity rider meet-and-greets</span>
                        </li>
                        <li>
                            <span class="check">✓</span>
                            <span>Premium catering and entertainment</span>
                        </li>
                        <li>
                            <span class="check">✓</span>
                            <span>IATSE Local 631 production crews</span>
                        </li>
                        <li>
                            <span class="check">✓</span>
                            <span>Brand activation and sponsorship integration</span>
                        </li>
                    </ul>
                    <div class="service-pricing gradient-text">
                        $75K - $500K
                    </div>
                    <div style="color: rgba(255,255,255,0.5); font-size: 13px; margin-bottom: 32px; letter-spacing: 1px;">
                        PER EVENT
                    </div>
                    <a href="#contact" class="btn btn-secondary" style="width: 100%;">Request Proposal</a>
                </div>

                <!-- VIP Membership -->
                <div class="service-card">
                    <div class="service-number">02</div>
                    <h3>The Paddock Club</h3>
                    <p style="color: rgba(255,255,255,0.6); margin: 20px 0 32px; font-size: 15px;">
                        Exclusive membership for ultra-high-net-worth individuals seeking elite access and experiences
                    </p>
                    <ul class="service-features">
                        <li>
                            <span class="check">✓</span>
                            <span>Private VIP lounge at all WEC events</span>
                        </li>
                        <li>
                            <span class="check">✓</span>
                            <span>Priority seating and parking</span>
                        </li>
                        <li>
                            <span class="check">✓</span>
                            <span>Behind-the-scenes barn tours</span>
                        </li>
                        <li>
                            <span class="check">✓</span>
                            <span>Member-only networking events</span>
                        </li>
                        <li>
                            <span class="check">✓</span>
                            <span>Concierge service for equine needs</span>
                        </li>
                    </ul>
                    <div class="service-pricing gradient-text">
                        $25K - $75K
                    </div>
                    <div style="color: rgba(255,255,255,0.5); font-size: 13px; margin-bottom: 32px; letter-spacing: 1px;">
                        ANNUAL MEMBERSHIP
                    </div>
                    <a href="#contact" class="btn btn-secondary" style="width: 100%;">Apply for Membership</a>
                </div>

                <!-- Elite Rider -->
                <div class="service-card">
                    <div class="service-number">03</div>
                    <h3>Elite Rider Brand Management</h3>
                    <p style="color: rgba(255,255,255,0.6); margin: 20px 0 32px; font-size: 15px;">
                        Professional brand development and sponsorship procurement for Olympic and World Cup level riders
                    </p>
                    <ul class="service-features">
                        <li>
                            <span class="check">✓</span>
                            <span>Personal brand development</span>
                        </li>
                        <li>
                            <span class="check">✓</span>
                            <span>Sponsorship procurement (20% commission)</span>
                        </li>
                        <li>
                            <span class="check">✓</span>
                            <span>Social media management</span>
                        </li>
                        <li>
                            <span class="check">✓</span>
                            <span>PR and media relations</span>
                        </li>
                        <li>
                            <span class="check">✓</span>
                            <span>Contract negotiation</span>
                        </li>
                    </ul>
                    <div class="service-pricing gradient-text">
                        $5K - $15K
                    </div>
                    <div style="color: rgba(255,255,255,0.5); font-size: 13px; margin-bottom: 32px; letter-spacing: 1px;">
                        MONTHLY RETAINER
                    </div>
                    <a href="#contact" class="btn btn-secondary" style="width: 100%;">Partner With Us</a>
                </div>

                <!-- Premium Experiences -->
                <div class="service-card">
                    <div class="service-number">04</div>
                    <h3>Premium Hospitality Experiences</h3>
                    <p style="color: rgba(255,255,255,0.6); margin: 20px 0 32px; font-size: 15px;">
                        Curated one-of-a-kind experiences with Olympic riders and behind-the-scenes access
                    </p>
                    <ul class="service-features">
                        <li>
                            <span class="check">✓</span>
                            <span>"Day in the Life" with top riders</span>
                        </li>
                        <li>
                            <span class="check">✓</span>
                            <span>Private training sessions</span>
                        </li>
                        <li>
                            <span class="check">✓</span>
                            <span>Exclusive dinner experiences</span>
                        </li>
                        <li>
                            <span class="check">✓</span>
                            <span>Photography packages</span>
                        </li>
                        <li>
                            <span class="check">✓</span>
                            <span>Proposal and special occasion planning</span>
                        </li>
                    </ul>
                    <div class="service-pricing gradient-text">
                        $5K - $25K
                    </div>
                    <div style="color: rgba(255,255,255,0.5); font-size: 13px; margin-bottom: 32px; letter-spacing: 1px;">
                        PER EXPERIENCE
                    </div>
                    <a href="#contact" class="btn btn-secondary" style="width: 100%;">Book Experience</a>
                </div>
            </div>
        </div>
    </section>

    <!-- Testimonials -->
    <section id="testimonials" class="testimonials">
        <div class="container">
            <div class="section-header">
                <h2>Trusted by the Elite</h2>
                <p class="section-subtitle">
                    From Fortune 500 executives to Olympic champions
                </p>
            </div>

            <div class="testimonial-grid">
                <div class="testimonial-card">
                    <div class="quote">"</div>
                    <p class="testimonial-text">
                        Ocala Elite Experiences delivered an impeccable corporate event for our 200 top dealers. 
                        The IATSE crew was professional, the venue was stunning, and every detail was perfect.
                    </p>
                    <div style="font-weight: 600; margin-bottom: 4px;">Richard Morrison</div>
                    <div style="font-size: 13px; color: rgba(255,255,255,0.5);">VP Corporate Events, Mercedes-Benz USA</div>
                </div>

                <div class="testimonial-card">
                    <div class="quote">"</div>
                    <p class="testimonial-text">
                        The Paddock Club membership has connected me with an incredible network of horse owners 
                        and industry leaders. The exclusive events are always first-class.
                    </p>
                    <div style="font-weight: 600; margin-bottom: 4px;">Alexandra Wellington</div>
                    <div style="font-size: 13px; color: rgba(255,255,255,0.5);">Platinum Member, Palm Beach</div>
                </div>

                <div class="testimonial-card">
                    <div class="quote">"</div>
                    <p class="testimonial-text">
                        Their brand management team secured me three major sponsorships within six months. 
                        Professional, connected, and they deliver results.
                    </p>
                    <div style="font-weight: 600; margin-bottom: 4px;">Sarah Chen</div>
                    <div style="font-size: 13px; color: rgba(255,255,255,0.5);">Olympic Show Jumper</div>
                </div>
            </div>
        </div>
    </section>

    <!-- CTA Section -->
    <section id="contact" class="cta-section">
        <div class="container">
            <div class="cta-content">
                <h2 style="color: white;">Ready to Experience Excellence?</h2>
                <p style="font-size: 1.3rem; margin: 32px 0 48px; color: rgba(255,255,255,0.7); font-weight: 300;">
                    Whether you're planning a corporate event, seeking exclusive membership, or looking for 
                    professional rider management, we invite you to discover the Ocala Elite difference.
                </p>
                <div style="display: flex; gap: 20px; justify-content: center; margin-bottom: 48px;">
                    <a href="mailto:events@ocalael ite.com" class="btn gradient-gold btn-primary" style="font-size: 16px;">
                        Schedule Consultation
                    </a>
                    <a href="#services" class="btn btn-secondary">
                        View Services
                    </a>
                </div>
                <div style="display: flex; gap: 48px; justify-content: center; color: rgba(255,255,255,0.6); font-size: 13px; text-transform: uppercase; letter-spacing: 1px;">
                    <div>◆ Private Consultations</div>
                    <div>◆ Custom Proposals</div>
                    <div>◆ White-Glove Service</div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-grid">
                <div>
                    <div class="logo-text gradient-text" style="margin-bottom: 24px;">Ocala Elite Experiences</div>
                    <p style="color: rgba(255,255,255,0.5); max-width: 300px; font-size: 14px; line-height: 1.8;">
                        Premium event production and hospitality at the World Equestrian Center. Where excellence meets elegance.
                    </p>
                </div>

                <div>
                    <h4 style="margin-bottom: 24px; font-weight: 600; font-size: 14px; letter-spacing: 1px;">Services</h4>
                    <ul class="footer-links">
                        <li><a href="#services">Corporate Events</a></li>
                        <li><a href="#services">The Paddock Club</a></li>
                        <li><a href="#services">Rider Management</a></li>
                        <li><a href="#services">Premium Experiences</a></li>
                    </ul>
                </div>

                <div>
                    <h4 style="margin-bottom: 24px; font-weight: 600; font-size: 14px; letter-spacing: 1px;">Company</h4>
                    <ul class="footer-links">
                        <li><a href="#testimonials">Testimonials</a></li>
                        <li><a href="#">Portfolio</a></li>
                        <li><a href="#">Press</a></li>
                        <li><a href="#">Careers</a></li>
                    </ul>
                </div>

                <div>
                    <h4 style="margin-bottom: 24px; font-weight: 600; font-size: 14px; letter-spacing: 1px;">Contact</h4>
                    <ul class="footer-links" style="color: rgba(255,255,255,0.5);">
                        <li>📧 events@ocalaelite.com</li>
                        <li>📞 (352) 555-ELITE</li>
                        <li>📍 World Equestrian Center</li>
                        <li>⏰ Available 24/7</li>
                    </ul>
                </div>
            </div>

            <div class="footer-bottom">
                <p>&copy; 2024 Ocala Elite Experiences. All rights reserved. IATSE Local 631 Partner.</p>
            </div>
        </div>
    </footer>

    <script>
        // Smooth scrolling
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({ behavior: 'smooth', block: 'start' });
                }
            });
        });
    </script>
</body>
</html>
