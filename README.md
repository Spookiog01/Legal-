<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <meta name="theme-color" content="#1e3a8a" />
    <meta name="description" content="Elite Private Investigation Services - Professional evidence gathering, surveillance, and legal documentation for harassment cases and targeted individuals." />
    <meta property="og:title" content="Elite Investigations - Professional Private Detective Services" />
    <meta property="og:description" content="Expert private investigation services with cutting-edge technology. Story submission, consultation booking, and proven results for justice." />
    <title>Elite Investigations - Truth Revealed, Justice Served | Professional Private Detective Services</title>

    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">

    <style>
        :root {
            --navy: #1a1a2e;
            --dark-blue: #16213e;
            --royal: #0f3460;
            --crimson: #e94560;
            --gold: #f39c12;
            --gradient-bg: linear-gradient(135deg, #1a1a2e 0%, #16213e 50%, #0f3460 100%);
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', 'Roboto', sans-serif;
            background: var(--gradient-bg);
            color: white;
            scroll-behavior: smooth;
            line-height: 1.6;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* Utility Classes */
        .bg-navy { background-color: var(--navy); }
        .bg-dark-blue { background-color: var(--dark-blue); }
        .bg-royal { background-color: var(--royal); }
        .bg-crimson { background-color: var(--crimson); }
        .text-crimson { color: var(--crimson); }
        .text-gold { color: var(--gold); }

        /* Animations */
        .animate-fade-in {
            animation: fadeIn 0.8s ease-in-out;
        }

        .animate-slide-up {
            animation: slideUp 0.6s ease-out;
        }

        .animate-pulse-glow {
            animation: pulseGlow 2s ease-in-out infinite;
        }

        .animate-float {
            animation: float 3s ease-in-out infinite;
        }

        @keyframes fadeIn {
            0% { opacity: 0; transform: translateY(30px); }
            100% { opacity: 1; transform: translateY(0); }
        }

        @keyframes slideUp {
            0% { transform: translateY(50px); opacity: 0; }
            100% { transform: translateY(0); opacity: 1; }
        }

        @keyframes pulseGlow {
            0%, 100% { box-shadow: 0 0 20px rgba(233, 69, 96, 0.4); }
            50% { box-shadow: 0 0 40px rgba(233, 69, 96, 0.8); }
        }

        @keyframes float {
            0%, 100% { transform: translateY(0px); }
            50% { transform: translateY(-10px); }
        }

        /* Glass Effect */
        .glass-effect {
            background: rgba(255, 255, 255, 0.05);
            backdrop-filter: blur(15px);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }

        /* Card Hover Effects */
        .service-card, .story-card, .professional-card {
            transition: all 0.4s ease;
            position: relative;
            overflow: hidden;
            cursor: pointer;
        }

        .service-card:hover, .story-card:hover, .professional-card:hover {
            transform: translateY(-10px) scale(1.02);
            box-shadow: 0 25px 50px rgba(0, 0, 0, 0.4);
        }

        .service-card::before, .professional-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.1), transparent);
            transition: left 0.6s;
        }

        .service-card:hover::before, .professional-card:hover::before {
            left: 100%;
        }

        /* Form Styles */
        .form-input {
            width: 100%;
            padding: 15px;
            background: var(--navy);
            border: 2px solid var(--royal);
            border-radius: 10px;
            color: white;
            font-size: 16px;
            transition: all 0.3s ease;
        }

        .form-input:focus {
            outline: none;
            border-color: var(--crimson);
            box-shadow: 0 0 15px rgba(233, 69, 96, 0.3);
        }

        .btn-primary {
            background: var(--crimson);
            color: white;
            padding: 15px 30px;
            border: none;
            border-radius: 10px;
            font-size: 16px;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s ease;
            text-decoration: none;
            display: inline-block;
            text-align: center;
        }

        .btn-primary:hover {
            background: #d63652;
            transform: translateY(-2px);
            box-shadow: 0 10px 25px rgba(233, 69, 96, 0.4);
        }

        .btn-secondary {
            background: transparent;
            color: white;
            padding: 15px 30px;
            border: 2px solid white;
            border-radius: 10px;
            font-size: 16px;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s ease;
            text-decoration: none;
            display: inline-block;
            text-align: center;
        }

        .btn-secondary:hover {
            background: white;
            color: var(--navy);
            transform: translateY(-2px);
        }

        /* Navigation */
        .navbar {
            background: rgba(22, 33, 62, 0.95);
            backdrop-filter: blur(15px);
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            padding: 15px 0;
            border-bottom: 1px solid rgba(255, 255, 255, 0.1);
        }

        .nav-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            display: flex;
            align-items: center;
            gap: 12px;
            font-size: 24px;
            font-weight: 800;
            color: white;
            text-decoration: none;
        }

        .logo-icon {
            width: 40px;
            height: 40px;
            background: var(--crimson);
            border-radius: 8px;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .nav-links {
            display: flex;
            gap: 30px;
            align-items: center;
        }

        .nav-links a {
            color: rgba(255, 255, 255, 0.8);
            text-decoration: none;
            font-weight: 500;
            transition: all 0.3s ease;
            position: relative;
        }

        .nav-links a:hover {
            color: var(--crimson);
        }

        .nav-links a::after {
            content: '';
            position: absolute;
            bottom: -5px;
            left: 0;
            width: 0;
            height: 2px;
            background: var(--crimson);
            transition: width 0.3s ease;
        }

        .nav-links a:hover::after {
            width: 100%;
        }

        /* Mobile Menu */
        .mobile-menu-btn {
            display: none;
            background: none;
            border: none;
            color: white;
            font-size: 24px;
            cursor: pointer;
        }

        /* Hero Section */
        .hero {
            min-height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            position: relative;
            overflow: hidden;
            background: url('https://images.unsplash.com/photo-1454165804606-c3d57bc86b40?ixlib=rb-4.0.3&auto=format&fit=crop&w=1920&h=1080') center/cover;
        }

        .hero::before {
            content: '';
            position: absolute;
            inset: 0;
            background: linear-gradient(135deg, rgba(26, 26, 46, 0.95) 0%, rgba(22, 33, 62, 0.85) 50%, rgba(15, 52, 96, 0.75) 100%);
        }

        .hero-content {
            position: relative;
            z-index: 10;
            text-align: center;
            max-width: 1000px;
            padding: 0 20px;
        }

        .hero h1 {
            font-size: clamp(3rem, 8vw, 6rem);
            font-weight: 800;
            margin-bottom: 30px;
            line-height: 1.1;
        }

        .hero .highlight {
            color: var(--crimson);
            display: block;
            animation: pulse 2s ease-in-out infinite;
        }

        .hero p {
            font-size: clamp(1.1rem, 3vw, 1.5rem);
            margin-bottom: 40px;
            color: rgba(255, 255, 255, 0.9);
            max-width: 800px;
            margin-left: auto;
            margin-right: auto;
        }

        .hero-buttons {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
            justify-content: center;
            margin-bottom: 40px;
        }

        .scroll-indicator {
            position: absolute;
            bottom: 30px;
            left: 50%;
            transform: translateX(-50%);
            animation: bounce 2s infinite;
        }

        @keyframes bounce {
            0%, 20%, 50%, 80%, 100% { transform: translateX(-50%) translateY(0); }
            40% { transform: translateX(-50%) translateY(-10px); }
            60% { transform: translateX(-50%) translateY(-5px); }
        }

        /* Section Styles */
        .section {
            padding: 100px 0;
        }

        .section-header {
            text-align: center;
            margin-bottom: 80px;
        }

        .section-header h2 {
            font-size: clamp(2.5rem, 6vw, 4rem);
            font-weight: 800;
            margin-bottom: 20px;
        }

        .section-header p {
            font-size: 1.2rem;
            color: rgba(255, 255, 255, 0.8);
            max-width: 700px;
            margin: 0 auto;
        }

        /* Grid Layouts */
        .grid {
            display: grid;
            gap: 30px;
        }

        .grid-2 { grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); }
        .grid-3 { grid-template-columns: repeat(auto-fit, minmax(350px, 1fr)); }

        /* Card Styles */
        .card {
            background: var(--dark-blue);
            border-radius: 20px;
            padding: 40px;
            border: 1px solid rgba(255, 255, 255, 0.1);
        }

        .card-icon {
            width: 60px;
            height: 60px;
            background: var(--crimson);
            border-radius: 15px;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-bottom: 25px;
        }

        .card h3 {
            font-size: 1.5rem;
            font-weight: 700;
            margin-bottom: 15px;
        }

        .card p {
            color: rgba(255, 255, 255, 0.8);
            margin-bottom: 25px;
        }

        .card img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 12px;
        }

        /* Professional Services Special Styling */
        .professional-services {
            background: linear-gradient(135deg, var(--royal) 0%, var(--navy) 100%);
        }

        .professional-card {
            background: linear-gradient(135deg, rgba(233, 69, 96, 0.1) 0%, rgba(255, 255, 255, 0.05) 100%);
            border: 2px solid rgba(233, 69, 96, 0.3);
        }

        .professional-card:hover {
            border-color: var(--crimson);
            box-shadow: 0 0 30px rgba(233, 69, 96, 0.4);
        }

        /* Story Submission Form */
        .story-form {
            background: var(--dark-blue);
            border-radius: 25px;
            padding: 50px;
            border: 1px solid rgba(255, 255, 255, 0.1);
            position: relative;
        }

        .step-indicator {
            margin-bottom: 40px;
        }

        .step-progress {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 15px;
        }

        .progress-bar {
            width: 100%;
            height: 8px;
            background: var(--royal);
            border-radius: 10px;
            overflow: hidden;
        }

        .progress-fill {
            height: 100%;
            background: linear-gradient(90deg, var(--crimson) 0%, var(--gold) 100%);
            transition: width 0.5s ease;
            border-radius: 10px;
        }

        .form-step {
            display: none;
        }

        .form-step.active {
            display: block;
            animation: fadeIn 0.5s ease;
        }

        .form-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            margin-bottom: 25px;
        }

        .form-group {
            margin-bottom: 25px;
        }

        .form-label {
            display: block;
            margin-bottom: 8px;
            font-weight: 600;
            color: rgba(255, 255, 255, 0.9);
        }

        .checkbox-group {
            display: grid;
            gap: 12px;
        }

        .checkbox-item {
            display: flex;
            align-items: center;
            gap: 12px;
            padding: 12px;
            background: rgba(255, 255, 255, 0.05);
            border-radius: 8px;
            cursor: pointer;
            transition: all 0.3s ease;
        }

        .checkbox-item:hover {
            background: rgba(233, 69, 96, 0.1);
        }

        .form-navigation {
            display: flex;
            justify-content: space-between;
            margin-top: 40px;
        }

        /* Consultation Section */
        .consultation-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 50px;
            align-items: start;
        }

        .time-slots {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 12px;
            margin-top: 15px;
        }

        .time-slot {
            padding: 12px;
            background: var(--royal);
            border: 2px solid transparent;
            border-radius: 8px;
            text-align: center;
            cursor: pointer;
            transition: all 0.3s ease;
        }

        .time-slot:hover, .time-slot.selected {
            background: var(--crimson);
            border-color: var(--crimson);
        }

        .consultation-type {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 15px;
            margin-top: 15px;
        }

        .type-option {
            padding: 20px;
            background: var(--navy);
            border: 2px solid var(--royal);
            border-radius: 12px;
            text-align: center;
            cursor: pointer;
            transition: all 0.3s ease;
        }

        .type-option:hover, .type-option.selected {
            border-color: var(--crimson);
            background: rgba(233, 69, 96, 0.1);
        }

        /* Testimonials */
        .testimonial-card {
            background: var(--dark-blue);
            border-radius: 20px;
            padding: 40px;
            position: relative;
            border: 1px solid rgba(255, 255, 255, 0.1);
        }

        .testimonial-card::before {
            content: '"';
            position: absolute;
            top: 20px;
            left: 20px;
            font-size: 60px;
            color: rgba(233, 69, 96, 0.3);
            font-weight: bold;
        }

        .testimonial-content {
            position: relative;
            z-index: 2;
        }

        .testimonial-text {
            font-style: italic;
            margin-bottom: 25px;
            color: rgba(255, 255, 255, 0.9);
        }

        .testimonial-author {
            display: flex;
            align-items: center;
            gap: 15px;
        }

        .author-avatar {
            width: 50px;
            height: 50px;
            border-radius: 50%;
            object-fit: cover;
        }

        .author-info h4 {
            font-weight: 600;
            margin-bottom: 5px;
        }

        .author-info span {
            color: var(--crimson);
            font-size: 0.9rem;
        }

        .stars {
            display: flex;
            gap: 5px;
            margin-top: 15px;
        }

        .star {
            color: var(--gold);
        }

        /* Footer */
        .footer {
            background: var(--dark-blue);
            padding: 80px 0 30px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
        }

        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 40px;
            margin-bottom: 40px;
        }

        .footer-section h3 {
            font-size: 1.3rem;
            font-weight: 700;
            margin-bottom: 20px;
        }

        .footer-links {
            list-style: none;
            padding: 0;
        }

        .footer-links li {
            margin-bottom: 12px;
        }

        .footer-links a {
            color: rgba(255, 255, 255, 0.7);
            text-decoration: none;
            transition: color 0.3s ease;
        }

        .footer-links a:hover {
            color: var(--crimson);
        }

        .contact-info {
            display: flex;
            align-items: center;
            gap: 12px;
            margin-bottom: 12px;
        }

        .social-links {
            display: flex;
            gap: 15px;
            margin-top: 20px;
        }

        .social-link {
            width: 40px;
            height: 40px;
            background: var(--royal);
            border-radius: 8px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            text-decoration: none;
            transition: all 0.3s ease;
        }

        .social-link:hover {
            background: var(--crimson);
            transform: translateY(-3px);
        }

        .footer-bottom {
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            padding-top: 30px;
            text-align: center;
            color: rgba(255, 255, 255, 0.6);
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .nav-links {
                display: none;
            }

            .mobile-menu-btn {
                display: block;
            }

            .hero-buttons {
                flex-direction: column;
                align-items: center;
            }

            .consultation-grid {
                grid-template-columns: 1fr;
                gap: 30px;
            }

            .time-slots {
                grid-template-columns: repeat(2, 1fr);
            }

            .consultation-type {
                grid-template-columns: 1fr;
            }

            .story-form {
                padding: 30px 20px;
            }

            .form-navigation {
                flex-direction: column;
                gap: 15px;
            }
        }

        @media (max-width: 480px) {
            .card {
                padding: 25px;
            }

            .section {
                padding: 60px 0;
            }

            .time-slots {
                grid-template-columns: 1fr;
            }
        }

        /* Custom Scrollbar */
        ::-webkit-scrollbar {
            width: 8px;
        }

        ::-webkit-scrollbar-track {
            background: var(--navy);
        }

        ::-webkit-scrollbar-thumb {
            background: var(--crimson);
            border-radius: 4px;
        }

        ::-webkit-scrollbar-thumb:hover {
            background: #d63652;
        }
    </style>
</head>
<body>
    <!-- Navigation -->
    <nav class="navbar">
        <div class="container">
            <div class="nav-content">
                <a href="#" class="logo">
                    <div class="logo-icon animate-pulse-glow">
                        🛡️
                    </div>
                    Elite Investigations
                </a>

                <div class="nav-links">
                    <a href="#services">Services</a>
                    <a href="#stories">Share Story</a>
                    <a href="#professional-services">Professional Services</a>
                    <a href="#consultation">Consultation</a>
                    <a href="#testimonials">About</a>
                    <a href="#contact" class="btn-primary">Get Help Now</a>
                </div>

                <button class="mobile-menu-btn">☰</button>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section class="hero animate-fade-in">
        <div class="hero-content">
            <h1>
                Truth Revealed
                <span class="highlight">Justice Served</span>
            </h1>
            <p>
                Professional private investigation services with cutting-edge technology and decades of experience. 
                From harassment documentation to corporate security, we deliver results that matter for targeted individuals seeking justice.
            </p>
            <div class="hero-buttons">
                <a href="#consultation" class="btn-primary animate-pulse-glow">Start Free Consultation</a>
                <a href="#stories" class="btn-secondary">Share Your Story</a>
                <a href="#professional-services" class="btn-primary" style="background: var(--gold);">Professional Services</a>
            </div>
        </div>
        <div class="scroll-indicator">
            <svg width="24" height="24" fill="white" viewBox="0 0 24 24">
                <path d="M7 10l5 5 5-5z"/>
            </svg>
        </div>
    </section>

    <!-- Services Section -->
    <section id="services" class="section bg-dark-blue">
        <div class="container">
            <div class="section-header animate-slide-up">
                <h2>Professional Investigation Services</h2>
                <p>Comprehensive investigation services backed by advanced technology and proven methodologies</p>
            </div>

            <div class="grid grid-3">
                <div class="service-card card animate-slide-up">
                    <div class="card-icon">
                        🔍
                    </div>
                    <h3>Background Investigations</h3>
                    <p>Comprehensive background checks for personal, professional, and legal purposes with detailed reporting and verification.</p>
                    <img src="https://images.unsplash.com/photo-1507003211169-0a1dd7228f2d?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&h=400" alt="Background Investigation">
                </div>

                <div class="service-card card animate-slide-up">
                    <div class="card-icon">
                        📹
                    </div>
                    <h3>Surveillance Operations</h3>
                    <p>Discreet surveillance services using state-of-the-art equipment and professional techniques for evidence gathering.</p>
                    <img src="https://images.unsplash.com/photo-1550751827-4bd374c3f58b?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&h=400" alt="Surveillance">
                </div>

                <div class="service-card card animate-slide-up">
                    <div class="card-icon">
                        ⚖️
                    </div>
                    <h3>Legal Support Services</h3>
                    <p>Expert witness testimony, evidence collection, and litigation support for legal proceedings and court cases.</p>
                    <img src="https://images.unsplash.com/photo-1589829545856-d10d557cf95f?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&h=400" alt="Legal Support">
                </div>

                <div class="service-card card animate-slide-up">
                    <div class="card-icon">
                        🛡️
                    </div>
                    <h3>Corporate Security</h3>
                    <p>Asset protection, employee misconduct investigations, and corporate intelligence services for businesses.</p>
                    <img src="https://images.unsplash.com/photo-1486312338219-ce68d2c6f44d?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&h=400" alt="Corporate Security">
                </div>

                <div class="service-card card animate-slide-up">
                    <div class="card-icon">
                        💝
                    </div>
                    <h3>Personal Matters</h3>
                    <p>Sensitive personal investigations including infidelity, missing persons, and family matters handled with discretion.</p>
                    <img src="https://images.unsplash.com/photo-1556157382-97eda2d62296?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&h=400" alt="Personal Matters">
                </div>

                <div class="service-card card animate-slide-up">
                    <div class="card-icon">
                        💻
                    </div>
                    <h3>Digital Forensics</h3>
                    <p>Advanced digital investigation services including data recovery, cyber crime analysis, and electronic evidence preservation.</p>
                    <img src="https://images.unsplash.com/photo-1563986768609-322da13575f3?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&h=400" alt="Digital Forensics">
                </div>
            </div>
        </div>
    </section>

    <!-- Professional Services for Targeted Individuals -->
    <section id="professional-services" class="section professional-services">
        <div class="container">
            <div class="section-header animate-slide-up">
                <h2>Professional Services for Targeted Individuals</h2>
                <p>Specialized investigation services designed to help individuals who are being targeted, harassed, or need evidence to pursue legal action and achieve justice.</p>
            </div>

            <div class="grid grid-2">
                <div class="professional-card card animate-slide-up">
                    <div class="card-icon">
                        📋
                    </div>
                    <h3>Harassment Documentation</h3>
                    <p>Comprehensive documentation of harassment incidents with legal validity. We gather, preserve, and present evidence in court-ready formats for restraining orders and legal proceedings.</p>
                    <img src="https://images.unsplash.com/photo-1544717297-fa95b6ee9643?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&h=400" alt="Harassment Documentation">
                </div>

                <div class="professional-card card animate-slide-up">
                    <div class="card-icon">
                        🎯
                    </div>
                    <h3>Evidence Gathering Against Specific Individuals</h3>
                    <p>Professional evidence collection targeting specific individuals involved in harassment, stalking, or other illegal activities. Surveillance, documentation, and witness interviews.</p>
                    <img src="https://images.unsplash.com/photo-1500389723459-ca24a5564899?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&h=400" alt="Evidence Gathering">
                </div>

                <div class="professional-card card animate-slide-up">
                    <div class="card-icon">
                        📱
                    </div>
                    <h3>Digital Harassment Investigation</h3>
                    <p>Investigation of cyberbullying, online harassment, and digital stalking. We trace digital footprints, preserve electronic evidence, and identify perpetrators.</p>
                    <img src="https://images.unsplash.com/photo-1563986768494-4dee2763ff3f?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&h=400" alt="Digital Investigation">
                </div>

                <div class="professional-card card animate-slide-up">
                    <div class="card-icon">
                        🏛️
                    </div>
                    <h3>Court Preparation & Legal Support</h3>
                    <p>Expert preparation for legal proceedings including evidence presentation, witness testimony, and collaboration with legal counsel to strengthen your case.</p>
                    <img src="https://images.unsplash.com/photo-1589829545856-d10d557cf95f?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&h=400" alt="Court Preparation">
                </div>

                <div class="professional-card card animate-slide-up">
                    <div class="card-icon">
                        🚨
                    </div>
                    <h3>Emergency Response Services</h3>
                    <p>24/7 emergency documentation and evidence collection for urgent situations. Immediate response for restraining order applications and emergency legal needs.</p>
                    <img src="https://images.unsplash.com/photo-1551601651-2a8555f1a136?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&h=400" alt="Emergency Response">
                </div>

                <div class="professional-card card animate-slide-up">
                    <div class="card-icon">
                        🔒
                    </div>
                    <h3>Confidential Consultation</h3>
                    <p>Completely confidential consultation services with attorney-client privilege protection. Safe space to discuss your situation and develop an action plan.</p>
                    <img src="https://images.unsplash.com/photo-1556155092-8707de31f9c4?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&h=400" alt="Confidential Consultation">
                </div>
            </div>

            <div style="text-align: center; margin-top: 60px;">
                <div style="background: rgba(233, 69, 96, 0.1); border: 2px solid var(--crimson); border-radius: 20px; padding: 40px; max-width: 800px; margin: 0 auto;">
                    <h3 style="color: var(--crimson); margin-bottom: 20px;">🔥 Emergency Hotline Available 24/7</h3>
                    <p style="margin-bottom: 25px;">If you're experiencing immediate harassment or need urgent evidence collection, our emergency response team is available around the clock.</p>
                    <div style="display: flex; gap: 20px; justify-content: center; flex-wrap: wrap;">
                        <a href="tel:(209)565-1438" class="btn-primary">📞 Call Emergency Line</a>
                        <a href="#consultation" class="btn-secondary" style="border-color: var(--crimson); color: var(--crimson);">Book Urgent Consultation</a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Interactive Story Submission -->
    <section id="stories" class="section bg-navy">
        <div class="container">
            <div class="section-header animate-slide-up">
                <h2>Share Your Story</h2>
                <p>Your story matters. Share your experience confidentially and let us help you find the truth and seek justice.</p>
            </div>

            <div style="max-width: 900px; margin: 0 auto;">
                <form class="story-form glass-effect" id="storySubmissionForm">
                    <!-- Step Indicator -->
                    <div class="step-indicator">
                        <div class="step-progress">
                            <span style="font-weight: 600;">Step <span id="currentStep">1</span> of 3</span>
                            <span style="font-weight: 600;"><span id="progressPercent">33</span>% Complete</span>
                        </div>
                        <div class="progress-bar">
                            <div class="progress-fill" id="progressFill" style="width: 33%;"></div>
                        </div>
                    </div>

                    <!-- Step 1: Basic Information -->
                    <div class="form-step active" id="step1">
                        <h3 style="font-size: 2rem; margin-bottom: 30px;">Tell Us About Your Situation</h3>

                        <div class="form-grid">
                            <div class="form-group">
                                <label class="form-label">Full Name *</label>
                                <input type="text" class="form-input" id="fullName" required>
                            </div>
                            <div class="form-group">
                                <label class="form-label">Email Address *</label>
                                <input type="email" class="form-input" id="email" required>
                            </div>
                        </div>

                        <div class="form-group">
                            <label class="form-label">Phone Number</label>
                            <input type="tel" class="form-input" id="phone">
                        </div>

                        <div class="form-group">
                            <label class="form-label">Story Title *</label>
                            <input type="text" class="form-input" id="storyTitle" placeholder="Brief title for your case" required>
                        </div>
                    </div>

                    <!-- Step 2: Story Details -->
                    <div class="form-step" id="step2">
                        <h3 style="font-size: 2rem; margin-bottom: 30px;">Case Details</h3>

                        <div class="form-grid">
