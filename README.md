    <!DOCTYPE html>
    <html lang="id">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>PRASTKAKIKAKI | Bengkel Spesialis Kaki-Kaki Profesional</title>
        <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
        <style>
            
            /* ==== GLOBAL STYLES ==== */
            :root {
                --primary: #0066ff; /* Neon Blue */
                --secondary: #e0e0e0; /* Silver */
                --dark: #0a0a0a; /* Black */
                --accent: #00ffcc; /* Teal */
                --text: #ffffff;
            }
            
            * {
                margin: 0;
                padding: 0;
                box-sizing: border-box;
                font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            }
            
            body {
                background-color: var(--dark);
                color: var(--text);
                line-height: 1.6;
                overflow-x: hidden;
            }
            
            .container {
                max-width: 1200px;
                margin: 0 auto;
                padding: 0 20px;
            }
            
            section {
                padding: 80px 0;
                border-bottom: 1px solid rgba(255,255,255,0.1);
            }
            
            h1, h2, h3 {
                margin-bottom: 20px;
            }
            
            h1 {
                font-size: 3.5rem;
                background: linear-gradient(90deg, var(--primary), var(--accent));
                -webkit-background-clip: text;
                background-clip: text;
                color: transparent;
            }
            
            h2 {
                font-size: 2.5rem;
                color: var(--secondary);
            }
            
            .btn {
                display: inline-block;
                padding: 15px 35px;
                background: var(--primary);
                color: white;
                text-decoration: none;
                border-radius: 50px;
                font-weight: bold;
                text-transform: uppercase;
                letter-spacing: 1px;
                transition: all 0.3s;
                border: none;
                cursor: pointer;
                font-size: 1.1rem;
                box-shadow: 0 0 15px rgba(0, 102, 255, 0.5);
            }
            
            .btn:hover {
                background: var(--accent);
                transform: translateY(-3px);
                box-shadow: 0 0 20px rgba(0, 255, 204, 0.7);
                color: var(--dark);
            }
            
            /* ==== HEADER ==== */
            header {
                background: rgba(10, 10, 10, 0.9);
                backdrop-filter: blur(10px);
                position: fixed;
                width: 100%;
                z-index: 1000;
                border-bottom: 1px solid rgba(255,255,255,0.1);
            }
            
            nav {
                display: flex;
                justify-content: space-between;
                align-items: center;
                padding: 20px 0;
            }
            
            .logo {
                font-size: 1.8rem;
                font-weight: 800;
                color: var(--primary);
                text-transform: uppercase;
            }
            
            .logo span {
                color: var(--secondary);
            }
            
            .nav-links {
                display: flex;
                list-style: none;
            }
            
            .nav-links li {
                margin-left: 30px;
            }
            
            .nav-links a {
                text-decoration: none;
                color: var(--secondary);
                font-weight: 600;
                transition: color 0.3s;
                position: relative;
            }
            
            .nav-links a:hover {
                color: var(--accent);
            }
            
            .nav-links a:after {
                content: '';
                position: absolute;
                width: 0;
                height: 2px;
                background: var(--accent);
                bottom: -5px;
                left: 0;
                transition: width 0.3s;
            }
            
            .nav-links a:hover:after {
                width: 100%;
            }
            
            /* ==== HERO ==== */
            .hero {
                background: linear-gradient(rgba(0,0,0,0.7), rgba(0,0,0,0.7)), url('https://images.unsplash.com/photo-1593941707882-a5bbbfd6d0b4?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80');
                background-size: cover;
                background-position: center;
                height: 100vh;
                display: flex;
                align-items: center;
                text-align: center;
            }
            
            .hero-content {
                max-width: 800px;
                margin: 0 auto;
            }
            
            .hero h1 {
                margin-bottom: 30px;
                line-height: 1.2;
            }
            
            .hero p {
                font-size: 1.2rem;
                margin-bottom: 40px;
                color: var(--secondary);
            }
            
            .cta-buttons {
                display: flex;
                justify-content: center;
                gap: 20px;
            }
            
            .btn-secondary {
                background: transparent;
                border: 2px solid var(--primary);
                color: var(--primary);
            }
            
            .btn-secondary:hover {
                background: transparent;
                border-color: var(--accent);
                color: var(--accent);
            }
            
            /* ==== TESTIMONIALS ==== */
            .testimonials {
                text-align: center;
            }
            
            .testimonial-grid {
                display: grid;
                grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
                gap: 30px;
                margin-top: 50px;
            }
            
            .testimonial-card {
                background: rgba(30, 30, 30, 0.7);
                padding: 30px;
                border-radius: 10px;
                border-left: 3px solid var(--primary);
                text-align: left;
                transition: transform 0.3s;
            }
            
            .testimonial-card:hover {
                transform: translateY(-10px);
                background: rgba(40, 40, 40, 0.9);
            }
            
            .testimonial-text {
                font-style: italic;
                margin-bottom: 20px;
                color: var(--secondary);
            }
            
            .testimonial-author {
                font-weight: bold;
                color: var(--accent);
            }
            
            /* ==== FEATURES ==== */
            .features {
                background: linear-gradient(rgba(10,10,10,0.9), rgba(10,10,10,0.9));
            }
            
            .features h2 {
                text-align: center;
                margin-bottom: 50px;
            }
            
            .features-grid {
                display: grid;
                grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
                gap: 30px;
            }
            
            .feature-card {
                background: rgba(20, 20, 20, 0.8);
                padding: 30px;
                border-radius: 10px;
                border-top: 3px solid var(--primary);
                transition: all 0.3s;
            }
            
            .feature-card:hover {
                transform: translateY(-10px);
                box-shadow: 0 10px 20px rgba(0,0,0,0.3);
                border-color: var(--accent);
            }
            
            .feature-icon {
                font-size: 2.5rem;
                color: var(--primary);
                margin-bottom: 20px;
            }
            
            .feature-card h3 {
                color: var(--secondary);
                font-size: 1.5rem;
            }
            
            /* ==== SERVICES ==== */
            .services ul {
                list-style: none;
                columns: 2;
                margin-top: 30px;
            }
            
            .services li {
                margin-bottom: 15px;
                position: relative;
                padding-left: 25px;
            }
            
            .services li:before {
                content: '\f00c';
                font-family: 'Font Awesome 6 Free';
                font-weight: 900;
                color: var(--accent);
                position: absolute;
                left: 0;
            }
            
    <!DOCTYPE html>
    <html lang="id">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>PRAST KAKI-KAKI | Bengkel Spesialis Premium</title>
        <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
        <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@300;400;500;600;700&display=swap" rel="stylesheet">
        <style>
            :root {
                --primary: #0066ff;
                --secondary: #e0e0e0;
                --dark: #0a0a0a;
                --accent: #00ffcc;
                --text: #ffffff;
                --bg-dark: #121212;
                --card-bg: #1e1e1e;
                --overlay: rgba(0, 22, 44, 0.85);
            }

            * {
                margin: 0;
                padding: 0;
                box-sizing: border-box;
                font-family: 'Montserrat', sans-serif;
            }

            body {
                background-color: var(--bg-dark);
                color: var(--text);
                line-height: 1.7;
                overflow-x: hidden;
                background-image: 
                    radial-gradient(circle at 20% 30%, rgba(0, 102, 255, 0.05) 0%, transparent 25%),
                    radial-gradient(circle at 80% 70%, rgba(0, 255, 204, 0.05) 0%, transparent 25%);
            }

            /* Header */
            header {
                background: rgba(15, 15, 15, 0.98);
                backdrop-filter: blur(10px);
                position: fixed;
                width: 100%;
                z-index: 1000;
                border-bottom: 1px solid rgba(0, 102, 255, 0.15);
                padding: 1.2rem 0;
            }

            nav {
                display: flex;
                justify-content: space-between;
                align-items: center;
                max-width: 1200px;
                margin: 0 auto;
                padding: 0 2rem;
            }

            .logo {
                font-size: 1.8rem;
                font-weight: 700;
                background: linear-gradient(90deg, var(--primary), var(--accent));
                -webkit-background-clip: text;
                background-clip: text;
                color: transparent;
                letter-spacing: 1px;
            }

            .nav-links {
                display: flex;
                list-style: none;
            }

            .nav-links li {
                margin-left: 2.5rem;
            }

            .nav-links a {
                color: var(--secondary);
                text-decoration: none;
                font-weight: 500;
                font-size: 0.95rem;
                letter-spacing: 0.5px;
                transition: all 0.3s;
                position: relative;
            }

            .nav-links a:hover {
                color: var(--accent);
            }

            .nav-links a::after {
                content: '';
                position: absolute;
                width: 0;
                height: 2px;
                background: var(--accent);
                bottom: -5px;
                left: 0;
                transition: width 0.3s;
            }

            .nav-links a:hover::after {
                width: 100%;
            }

            /* Hero Section */
            .hero {
                height: 100vh;
                display: flex;
                align-items: center;
                position: relative;
                overflow: hidden;
            }

            .hero::before {
                content: '';
                position: absolute;
                top: 0;
                left: 0;
                width: 100%;
                height: 100%;
                background: linear-gradient(rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0.7)), 
                            url('https://images.unsplash.com/photo-1593941707882-a5bbbfd6d0b4?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80');
                background-size: cover;
                background-position: center;
                z-index: -1;
            }

            .hero-content {
                max-width: 1200px;
                margin: 0 auto;
                padding: 0 2rem;
                position: relative;
                z-index: 1;
                text-align: center;
            }

            .hero h1 {
                font-size: 3.5rem;
                margin-bottom: 1.5rem;
                background: linear-gradient(90deg, var(--primary), var(--accent));
                -webkit-background-clip: text;
                background-clip: text;
                color: transparent;
                line-height: 1.2;
            }

            .hero p {
                font-size: 1.2rem;
                color: rgba(255, 255, 255, 0.8);
                max-width: 700px;
                margin: 0 auto 2rem;
            }

            .stats {
                background: rgba(0, 102, 255, 0.15);
                backdrop-filter: blur(5px);
                padding: 1.2rem;
                border-radius: 8px;
                display: inline-block;
                margin: 2rem 0;
                border: 1px solid rgba(0, 102, 255, 0.3);
            }

            .stats p {
                margin: 0;
                color: var(--accent);
                font-weight: 500;
            }

            .btn {
                display: inline-block;
                padding: 1rem 2.5rem;
                background: var(--primary);
                color: white;
                text-decoration: none;
                border-radius: 50px;
                font-weight: 600;
                text-transform: uppercase;
                letter-spacing: 1px;
                font-size: 0.95rem;
                transition: all 0.3s;
                box-shadow: 0 5px 20px rgba(0, 102, 255, 0.3);
                margin: 0.5rem;
            }

            .btn:hover {
                background: var(--accent);
                transform: translateY(-3px);
                box-shadow: 0 8px 25px rgba(0, 255, 204, 0.4);
                color: var(--dark);
            }

            .btn-secondary {
                background: transparent;
                border: 2px solid var(--primary);
                color: var(--primary);
            }

            .btn-secondary:hover {
                border-color: var(--accent);
                color: var(--accent);
                background: transparent;
            }

            /* Testimonials */
            .testimonials {
                padding: 6rem 0;
                background: linear-gradient(rgba(10, 10, 10, 0.95), rgba(10, 10, 10, 0.95));
            }

            .section-title {
                text-align: center;
                margin-bottom: 4rem;
            }

            .section-title h2 {
                font-size: 2.5rem;
                color: var(--secondary);
                margin-bottom: 1rem;
                position: relative;
                display: inline-block;
            }

            .section-title h2::after {
                content: '';
                position: absolute;
                width: 50%;
                height: 3px;
                background: linear-gradient(90deg, var(--primary), transparent);
                bottom: -10px;
                left: 25%;
            }

            .section-title p {
                color: rgba(255, 255, 255, 0.7);
                max-width: 700px;
                margin: 0 auto;
            }

            .testimonial-grid {
                display: grid;
                grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
                gap: 2rem;
                max-width: 1200px;
                margin: 0 auto;
                padding: 0 2rem;
            }

            .testimonial-card {
                background: var(--card-bg);
                padding: 2.5rem;
                border-radius: 12px;
                border-left: 3px solid var(--primary);
                transition: all 0.3s;
                box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
                position: relative;
                overflow: hidden;
            }

            .testimonial-card::before {
                content: '"';
                position: absolute;
                top: 1rem;
                right: 2rem;
                font-size: 5rem;
                color: rgba(0, 102, 255, 0.1);
                font-family: Georgia, serif;
                line-height: 1;
                z-index: 0;
            }

            .testimonial-card:hover {
                transform: translateY(-8px);
                box-shadow: 0 15px 40px rgba(0, 102, 255, 0.25);
                border-color: var(--accent);
            }

            .testimonial-text {
                font-style: italic;
                margin-bottom: 1.5rem;
                color: rgba(255, 255, 255, 0.9);
                position: relative;
                z-index: 1;
            }

            .testimonial-author {
                font-weight: 600;
                color: var(--accent);
                position: relative;
                z-index: 1;
            }

            /* Services */
            .services {
                padding: 6rem 0;
                position: relative;
            }

            .service-grid {
                display: grid;
                grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
                gap: 2rem;
                max-width: 1200px;
                margin: 0 auto;
                padding: 0 2rem;
            }

            .service-card {
                background: var(--card-bg);
                padding: 2.5rem;
                border-radius: 12px;
                border-top: 3px solid var(--primary);
                transition: all 0.3s;
                box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
                position: relative;
                overflow: hidden;
            }

            .service-card::before {
                content: '';
                position: absolute;
                top: 0;
                left: 0;
                width: 100%;
                height: 100%;
                background: linear-gradient(135deg, rgba(0, 102, 255, 0.05), transparent);
                z-index: 0;
            }

            .service-card:hover {
                transform: translateY(-10px);
                box-shadow: 0 15px 40px rgba(0, 102, 255, 0.25);
                border-color: var(--accent);
            }

            .service-icon {
                font-size: 2.5rem;
                color: var(--primary);
                margin-bottom: 1.5rem;
                position: relative;
                z-index: 1;
            }

            .service-card h3 {
                color: var(--secondary);
                margin-bottom: 1rem;
                position: relative;
                z-index: 1;
            }

            .price {
                font-size: 1.8rem;
                color: var(--accent);
                margin: 1.5rem 0;
                position: relative;
                z-index: 1;
            }

            .original-price {
                text-decoration: line-through;
                color: var(--secondary);
                opacity: 0.6;
                font-size: 1.2rem;
                margin-right: 0.8rem;
            }

            .service-features {
                list-style: none;
                margin: 1.5rem 0;
                position: relative;
                z-index: 1;
            }

            .service-features li {
                margin-bottom: 0.8rem;
                position: relative;
                padding-left: 1.8rem;
                color: rgba(255, 255, 255, 0.8);
            }

            .service-features li::before {
                content: '\f00c';
                font-family: 'Font Awesome 6 Free';
                font-weight: 900;
                color: var(--primary);
                position: absolute;
                left: 0;
                font-size: 0.9rem;
            }

            /* Guarantee */
            .guarantee {
                padding: 6rem 0;
                background: linear-gradient(135deg, rgba(0, 30, 60, 0.9), rgba(0, 0, 20, 0.9));
                text-align: center;
                position: relative;
                overflow: hidden;
            }

            .guarantee::before {
                content: '';
                position: absolute;
                top: -50%;
                left: -50%;
                width: 200%;
                height: 200%;
                background: radial-gradient(circle, rgba(0, 255, 204, 0.05) 0%, transparent 70%);
                animation: rotate 20s linear infinite;
                z-index: 0;
            }

            .guarantee-content {
                position: relative;
                z-index: 2;
                max-width: 800px;
                margin: 0 auto;
            }

            .guarantee-badge {
                background: var(--accent);
                color: var(--dark);
                padding: 0.5rem 1.5rem;
                border-radius: 50px;
                font-weight: 700;
                display: inline-block;
                margin-bottom: 2rem;
                font-size: 1.1rem;
                text-transform: uppercase;
                letter-spacing: 1px;
                box-shadow: 0 5px 15px rgba(0, 255, 204, 0.3);
            }

            .guarantee-list {
                list-style: none;
                text-align: left;
                display: inline-block;
                margin: 2rem 0;
            }

            .guarantee-list li {
                margin-bottom: 1rem;
                position: relative;
                padding-left: 2rem;
                color: rgba(255, 255, 255, 0.9);
            }

            .guarantee-list li::before {
                content: '\f058';
                font-family: 'Font Awesome 6 Free';
                font-weight: 900;
                color: var(--accent);
                position: absolute;
                left: 0;
                font-size: 1.2rem;
            }

            /* Locations */
            .locations {
                padding: 6rem 0;
                text-align: center;
            }

            .location-cards {
                display: grid;
                grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
                gap: 2rem;
                max-width: 1200px;
                margin: 0 auto;
                padding: 0 2rem;
            }

            .location-card {
                background: var(--card-bg);
                padding: 2rem;
                border-radius: 12px;
                transition: all 0.3s;
                border: 1px solid rgba(0, 102, 255, 0.2);
                box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
                position: relative;
                overflow: hidden;
            }

            .location-card::after {
                content: '';
                position: absolute;
                bottom: 0;
                left: 0;
                width: 100%;
                height: 4px;
                background: linear-gradient(90deg, var(--primary), var(--accent));
                transition: height 0.3s;
            }

            .location-card:hover {
                transform: translateY(-8px);
                box-shadow: 0 15px 40px rgba(0, 102, 255, 0.25);
            }

            .location-card:hover::after {
                height: 8px;
            }

            .location-card h3 {
                color: var(--primary);
                margin-bottom: 1rem;
            }

            .address {
                margin: 1rem 0;
                color: rgba(255, 255, 255, 0.8);
            }

            .map-link {
                display: inline-block;
                margin-top: 1rem;
                color: var(--accent);
                text-decoration: none;
                font-weight: 500;
                transition: all 0.3s;
            }

            .map-link:hover {
                text-decoration: underline;
            }

            /* Contact */
            .contact {
                padding: 6rem 0;
                background: var(--bg-dark);
                text-align: center;
            }

            .social-links {
                display: flex;
                justify-content: center;
                gap: 1.5rem;
                margin-top: 2rem;
                flex-wrap: wrap;
            }

            .social-link {
                width: 50px;
                height: 50px;
                border-radius: 50%;
                background: var(--card-bg);
                display: flex;
                align-items: center;
                justify-content: center;
                color: var(--secondary);
                font-size: 1.2rem;
                transition: all 0.3s;
                box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            }

            .social-link:hover {
                background: var(--primary);
                color: white;
                transform: translateY(-5px);
                box-shadow: 0 10px 20px rgba(0, 102, 255, 0.3);
            }

            /* Footer */
            footer {
                padding: 3rem 0;
                background: #080808;
                text-align: center;
                border-top: 1px solid rgba(0, 102, 255, 0.1);
            }

            .copyright {
                color: rgba(255, 255, 255, 0.5);
                font-size
            /* ==== CTA ==== */
            .cta {
                background: linear-gradient(135deg, var(--primary), var(--accent));
                text-align: center;
                padding: 100px 0;
            }
            
            .cta h2 {
                color: var(--dark);
                margin-bottom: 30px;
            }
            
            /* ==== FLOATING WHATSAPP BUTTON ==== */
            .floating-wa {
                position: fixed;
                bottom: 30px;
                right: 30px;
                background: #25D366;
                color: white;
                width: 60px;
                height: 60px;
                border-radius: 50%;
                display: flex;
                align-items: center;
                justify-content: center;
                font-size: 2rem;
                box-shadow: 0 5px 15px rgba(37, 211, 102, 0.5);
                z-index: 999;
                transition: all 0.3s;
                animation: pulse 2s infinite;
            }
            
            .floating-wa:hover {
                transform: scale(1.1);
                box-shadow: 0 8px 20px rgba(37, 211, 102, 0.7);
            }
            
            @keyframes pulse {
                0% { transform: scale(1); }
                50% { transform: scale(1.1); }
                100% { transform: scale(1); }
            }
            
            /* ==== FOOTER ==== */
            footer {
                background: #080808;
                padding: 50px 0 20px;
            }
            
            .footer-content {
                display: grid;
                grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
                gap: 30px;
                margin-bottom: 40px;
            }
            
            .footer-column h3 {
                color: var(--primary);
                margin-bottom: 20px;
                font-size: 1.3rem;
            }
            
            .footer-links {
                list-style: none;
            }
            
            .footer-links li {
                margin-bottom: 10px;
            }
            
            .footer-links a {
                color: var(--secondary);
                text-decoration: none;
                transition: color 0.3s;
            }
            
            .footer-links a:hover {
                color: var(--accent);
            }
            
            .social-links {
                display: flex;
                gap: 15px;
                margin-top: 20px;
            }
            
            .social-links a {
                color: var(--secondary);
                font-size: 1.5rem;
                transition: color 0.3s;
            }
            
            .social-links a:hover {
                color: var(--accent);
            }
            
            .copyright {
                text-align: center;
                padding-top: 20px;
                border-top: 1px solid rgba(255, 255, 255, 0.1);
                color: var(--secondary);
            }
            
            /* ==== RESPONSIVE ==== */
            @media (max-width: 768px) {
                h1 { font-size: 2.5rem; }
                h2 { font-size: 2rem; }
                
                .nav-links {
                    display: none;
                }
                
                .cta-buttons {
                    flex-direction: column;
                }
                
                .services ul {
                    columns: 1;
                }
            }
        </style>
    </head>
    <body>
        <!-- Floating WhatsApp Button -->
        <a href="https://wa.me/6281226298787" class="floating-wa" target="_blank">
            <i class="fab fa-whatsapp"></i>
        </a>

        <!-- Header -->
        <header>
            <div class="container">
                <nav>
                    <div class="logo">PR<span>AST KAKI KAKI</span></div>
                    <ul class="nav-links">
                        <li><a href="#testimonials">Testimoni</a></li>
                        <li><a href="#features">Keunggulan</a></li>
                        <li><a href="#services">Layanan</a></li>
                        <li><a href="#locations">Cabang</a></li>
                        <li><a href="#contact">Kontak</a></li>
                    </ul>
                </nav>
            </div>
        </header>

        <!-- Hero Section -->
        <section class="hero">
            <div class="container">
                <div class="hero-content">
                    <h1>Spesialis Servis Kaki-Kaki Mobil</h1>
                    <p>Ratusan mobil sudah mempercayakan perawatan kaki-kaki pada kami. Sekarang giliran Anda!</p>
                    <div class="cta-buttons">
                        <a href="https://wa.me/6281226298787" class="btn" target="_blank">Booking Sekarang</a>
                        <a href="#services" class="btn btn-secondary">Lihat Layanan</a>
                    </div>
                </div>
            </div>
        </section>

        <!-- Testimonials Section -->
        <section class="testimonials" id="testimonials">
            <div class="container">
                <h2>Apa Kata Pelanggan Kami</h2>
                <p>Bukti nyata kepuasan pelanggan</p>
                
                <div class="testimonial-grid">
                    <div class="testimonial-card">
                        <p class="testimonial-text">"Sudah langganan di Pras kaki. Kerjaannya sipp, harga juga miring. Cuma ada sparepart yang kosong tp masih bisa diakal sm montirnya. Klo kesini mendingan pagi biar ga ngantri banyak. Om Pras jg ramah. Bagusnya lg disini berani ngasik garansi satu tahun. Mantapp dah!"</p>
                        <p class="testimonial-author">- Haryanto Budiawan</p>
                    </div>
                    
                    <div class="testimonial-card">
                        <p class="testimonial-text">"Bengkel spesialis kaki-kaki yang recommended! Saya datang ke Prast Kaki Kaki bawa CR-V Gen karena ada bunyi di bagian suspensi dan setir terasa nggak stabil. Begitu dicek, langsung ketahuan masalahnya dan dijelaskan dengan detail. Mekaniknya berpengalaman nggak asal ganti part, dan pengerjaannya rapi. Setelah dikerjakan, mobil jadi jauh lebih nyaman dan stabil. Harganya juga masuk akal."</p>
                        <p class="testimonial-author">- Pak Freedy</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Features Section -->
        <section class="features" id="features">
            <div class="container">
                <h2>Keunggulan Prast Kaki-Kaki</h2>
                <p>Mengapa pelanggan memilih kami</p>
                
                <div class="features-grid">
                    <div class="feature-card">
                        <div class="feature-icon"><i class="fas fa-shield-alt"></i></div>
                        <h3>GARANSI 1 TAHUN</h3>
                        <p>Servis kaki-kaki dijamin satu tahun. Kalau ada masalah, balik ke kami, kami perbaiki GRATIS.</p>
                    </div>
                    
                    <div class="feature-card">
                        <div class="feature-icon"><i class="fas fa-tags"></i></div>
                        <h3>HARGA LEBIH MURAH</h3>
                        <p>Harga spare part & jasa lebih hemat dibanding bengkel resmi, kualitas sama premium.</p>
                    </div>
                    
                    <div class="feature-card">
                        <div class="feature-icon"><i class="fas fa-bolt"></i></div>
                        <h3>CEPAT! 3 JAM LANGSUNG JALAN</h3>
                        <p>Selesai hari ini juga, hanya 3 jam untuk servis standar. Mekanik banyak, antrian tidak perlu tunggu berhari-hari.</p>
                    </div>
                    
                    <div class="feature-card">
                        <div class="feature-icon"><i class="fas fa-gift"></i></div>
                        <h3>PROMO KHUSUS</h3>
                        <p>Konsultasi GRATIS dan ada promo Servis Rem & Spooring gratis khusus paket servis kaki kaki.</p>
                    </div>
        </section>
        
    <!DOCTYPE html>
    <html lang="id">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>PRAST KAKI KAKI | Bengkel Spesialis Kaki-Kaki Profesional</title>
        <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
        <style>
            /* ==== GLOBAL STYLES ==== */
            :root {
                --primary: #0066ff; /* Neon Blue */
                --secondary: #e0e0e0; /* Silver */
                --dark: #0a0a0a; /* Black */
                --accent: #00ffcc; /* Teal */
                --text: #ffffff;
            }
            
            * {
                margin: 0;
                padding: 0;
                box-sizing: border-box;
                font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            }
            
            body {
                background-color: var(--dark);
                color: var(--text);
                line-height: 1.6;
                overflow-x: hidden;
            }
            
            .container {
                max-width: 1200px;
                margin: 0 auto;
                padding: 0 20px;
            }
            
            section {
                padding: 80px 0;
                border-bottom: 1px solid rgba(255,255,255,0.1);
            }
            
            h1, h2, h3 {
                margin-bottom: 20px;
            }
            
            h1 {
                font-size: 3.5rem;
                background: linear-gradient(90deg, var(--primary), var(--accent));
                -webkit-background-clip: text;
                background-clip: text;
                color: transparent;
            }
            
            h2 {
                font-size: 2.5rem;
                color: var(--secondary);
            }
            
            .btn {
                display: inline-block;
                padding: 15px 35px;
                background: var(--primary);
                color: white;
                text-decoration: none;
                border-radius: 50px;
                font-weight: bold;
                text-transform: uppercase;
                letter-spacing: 1px;
                transition: all 0.3s;
                border: none;
                cursor: pointer;
                font-size: 1.1rem;
                box-shadow: 0 0 15px rgba(0, 102, 255, 0.5);
            }
            
            .btn:hover {
                background: var(--accent);
                transform: translateY(-3px);
                box-shadow: 0 0 20px rgba(0, 255, 204, 0.7);
                color: var(--dark);
            }
            
            /* ==== HEADER ==== */
            header {
                background: rgba(10, 10, 10, 0.9);
                backdrop-filter: blur(10px);
                position: fixed;
                width: 100%;
                z-index: 1000;
                border-bottom: 1px solid rgba(255,255,255,0.1);
            }
            
            nav {
                display: flex;
                justify-content: space-between;
                align-items: center;
                padding: 20px 0;
            }
            
            .logo {
                font-size: 1.8rem;
                font-weight: 800;
                color: var(--primary);
                text-transform: uppercase;
            }
            
            .logo span {
                color: var(--secondary);
            }
            
            .nav-links {
                display: flex;
                list-style: none;
            }
            
            .nav-links li {
                margin-left: 30px;
            }
            
            .nav-links a {
                text-decoration: none;
                color: var(--secondary);
                font-weight: 600;
                transition: color 0.3s;
                position: relative;
            }
            
            .nav-links a:hover {
                color: var(--accent);
            }
            
            .nav-links a:after {
                content: '';
                position: absolute;
                width: 0;
                height: 2px;
                background: var(--accent);
                bottom: -5px;
                left: 0;
                transition: width 0.3s;
            }
            
            .nav-links a:hover:after {
                width: 100%;
            }
            
            /* ==== HERO ==== */
            .hero {
                background: linear-gradient(rgba(0,0,0,0.7), rgba(0,0,0,0.7)), url('https://images.unsplash.com/photo-1593941707882-a5bbbfd6d0b4?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80');
                background-size: cover;
                background-position: center;
                height: 100vh;
                display: flex;
                align-items: center;
                text-align: center;
            }
            
            .hero-content {
                max-width: 800px;
                margin: 0 auto;
            }
            
            .hero h1 {
                margin-bottom: 30px;
                line-height: 1.2;
            }
            
            .hero p {
                font-size: 1.2rem;
                margin-bottom: 40px;
                color: var(--secondary);
            }
            
            .cta-buttons {
                display: flex;
                justify-content: center;
                gap: 20px;
            }
            
            .btn-secondary {
                background: transparent;
                border: 2px solid var(--primary);
                color: var(--primary);
            }
            
            .btn-secondary:hover {
                background: transparent;
                border-color: var(--accent);
                color: var(--accent);
            }
            
            /* ==== TESTIMONIALS ==== */
            .testimonials {
                text-align: center;
            }
            
            .testimonial-grid {
                display: grid;
                grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
                gap: 30px;
                margin-top: 50px;
            }
            
            .testimonial-card {
                background: rgba(30, 30, 30, 0.7);
                padding: 30px;
                border-radius: 10px;
                border-left: 3px solid var(--primary);
                text-align: left;
                transition: transform 0.3s;
            }
            
            .testimonial-card:hover {
                transform: translateY(-10px);
                background: rgba(40, 40, 40, 0.9);
            }
            
            .testimonial-text {
                font-style: italic;
                margin-bottom: 20px;
                color: var(--secondary);
            }
            
            .testimonial-author {
                font-weight: bold;
                color: var(--accent);
            }
            
            /* ==== SERVICES ==== */
            .services {
                text-align: center;
            }
            
            .service-grid {
                display: grid;
                grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
                gap: 30px;
                margin-top: 50px;
            }
            
            .service-card {
                background: rgba(20, 20, 20, 0.8);
                padding: 30px;
                border-radius: 10px;
                border-top: 3px solid var(--primary);
                transition: all 0.3s;
            }
            
            .service-card:hover {
                transform: translateY(-10px);
                box-shadow: 0 10px 20px rgba(0,0,0,0.3);
                border-color: var(--accent);
            }
            
            .service-card h3 {
                color: var(--secondary);
                font-size: 1.5rem;
                margin-bottom: 15px;
            }
            
            .service-price {
                font-size: 1.8rem;
                color: var(--accent);
                margin: 20px 0;
            }
            
            .service-features {
                list-style: none;
                text-align: left;
            }
            
            .service-features li {
                margin-bottom: 10px;
                position: relative;
                padding-left: 25px;
            }
            
            .service-features li:before {
                content: '\f00c';
                font-family: 'Font Awesome 6 Free';
                font-weight: 900;
                color: var(--accent);
                position: absolute;
                left: 0;
            }
            
            /* ==== LOCATIONS ==== */
            .locations {
                text-align: center;
            }
            
            .location-cards {
                display: grid;
                grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
                gap: 30px;
                margin-top: 50px;
            }
            
            .location-card {
                background: rgba(20, 20, 20, 0.8);
                padding: 30px;
                border-radius: 10px;
                transition: all 0.3s;
            }
            
            .location-card:hover {
                transform: translateY(-10px);
                box-shadow: 0 10px 20px rgba(0,0,0,0.3);
            }
            
            .location-card h3 {
                color: var(--primary);
                margin-bottom: 15px;
            }
            
            .location-address {
                margin-bottom: 15px;
                color: var(--secondary);
            }
            
            .location-link {
                color: var(--accent);
                text-decoration: none;
                font-weight: 600;
            }
            
            /* ==== CTA ==== */
            .cta {
                background: linear-gradient(135deg, var(--primary), var(--accent));
                text-align: center;
                padding: 100px 0;
            }
            
            .cta h2 {
                color: var(--dark);
                margin-bottom: 30px;
            }
            
            /* ==== CONTACT ==== */
            .contact {
                text-align: center;
            }
            
            .social-media {
                display: flex;
                justify-content: center;
                gap: 20px;
                margin-top: 30px;
            }
            
            .social-icon {
                width: 50px;
                height: 50px;
                border-radius: 50%;
                background: rgba(255,255,255,0.1);
                display: flex;
                align-items: center;
                justify-content: center;
                color: var(--secondary);
                font-size: 1.5rem;
                transition: all 0.3s;
            }
            
            .social-icon:hover {
                background: var(--primary);
                color: white;
                transform: translateY(-5px);
            }
            
            /* ==== FLOATING WHATSAPP BUTTON ==== */
            .floating-wa {
                position: fixed;
                bottom: 30px;
                right: 30px;
                background: #25D366;
                color: white;
                width: 60px;
                height: 60px;
                border-radius: 50%;
                display: flex;
                align-items: center;
                justify-content: center;
                font-size: 2rem;
                box-shadow: 0 5px 15px rgba(37, 211, 102, 0.5);
                z-index: 999;
                transition: all 0.3s;
                animation: pulse 2s infinite;
            }
            
            .floating-wa:hover {
                transform: scale(1.1);
                box-shadow: 0 8px 20px rgba(37, 211, 102, 0.7);
            }
            
            @keyframes pulse {
                0% { transform: scale(1); }
                50% { transform: scale(1.1); }
                100% { transform: scale(1); }
            }
            
            /* ==== FOOTER ==== */
            footer {
                background: #080808;
                padding: 50px 0 20px;
            }
            
            .footer-content {
                display: grid;
                grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
                gap: 30px;
                margin-bottom: 40px;
            }
            
            .footer-column h3 {
                color: var(--primary);
                margin-bottom: 20px;
                font-size: 1.3rem;
            }
            
            .footer-links {
                list-style: none;
            }
            
            .footer-links li {
                margin-bottom: 10px;
            }
            
            .footer-links a {
                color: var(--secondary);
                text-decoration: none;
                transition: color 0.3s;
            }
            
            .footer-links a:hover {
                color: var(--accent);
            }
            
            .social-links {
                display: flex;
                gap: 15px;
                margin-top: 20px;
            }
            
            .social-links a {
                color: var(--secondary);
                font-size: 1.5rem;
                transition: color 0.3s;
            }
            
            .social-links a:hover {
                color: var(--accent);
            }
            
            .copyright {
                text-align: center;
                padding-top: 20px;
                border-top: 1px solid rgba(255, 255, 255, 0.1);
                color: var(--secondary);
            }
            
            /* ==== RESPONSIVE ==== */
            @media (max-width: 768px) {
                h1 { font-size: 2.5rem; }
                h2 { font-size: 2rem; }
                
                .nav-links {
                    display: none;
                }
                
                .cta-buttons {
                    flex-direction: column;
                }
            }
        </style>
    </head>
    <body>
        
        <!-- Floating WhatsApp Button -->
        <a href="https://wa.me/6281226298787" class="floating-wa" target="_blank">
            <i class="fab fa-whatsapp"></i>
        </a>

        <!-- Header -->
        <header>
            <div class="container">
                <nav>
                    <div class="logo">PR<span>AST</span></div>
                    <ul class="nav-links">
                        <li><a href="#testimonials">Testimoni</a></li>
                        <li><a href="#services">Layanan</a></li>
                        <li><a href="#locations">Cabang</a></li>
                        <li><a href="#contact">Kontak</a></li>
                    </ul>
                </nav>
            </div>
        </header>

<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>PRAST KAKI KAKI - Layanan Profesional</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        /* Dark Theme Styles */
        :root {
            --primary: #3aa8ff;
            --primary-dark: #2e8acf;
            --dark-bg: #121212;
            --dark-card: #1e1e1e;
            --text-primary: #f5f5f5;
            --text-secondary: #b0b0b0;
            --accent: #ff6b6b;
        }
        
        body {
            background-color: var(--dark-bg);
            color: var(--text-primary);
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        .services {
            padding: 80px 0;
            background-color: var(--dark-bg);
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        .services h2 {
            text-align: center;
            font-size: 2.5rem;
            color: var(--text-primary);
            margin-bottom: 15px;
            position: relative;
        }
        
        .services h2::after {
            content: '';
            display: block;
            width: 80px;
            height: 4px;
            background: var(--primary);
            margin: 15px auto;
            border-radius: 2px;
        }
        
        .section-subtitle {
            text-align: center;
            color: var(--text-secondary);
            font-size: 1.1rem;
            margin-bottom: 50px;
        }
        
        .service-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }
        
        .service-card {
            background: var(--dark-card);
            border-radius: 12px;
            padding: 30px;
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.3);
            transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
            border: 1px solid #2a2a2a;
            position: relative;
            overflow: hidden;
        }
        
        .service-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.4);
            border-color: var(--primary);
        }
        
        .service-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(135deg, rgba(58, 168, 255, 0.1) 0%, rgba(0,0,0,0) 100%);
            z-index: 0;
        }
        
        .service-icon {
            font-size: 2.5rem;
            color: var(--primary);
            margin-bottom: 20px;
            text-align: center;
            position: relative;
        }
        
        .service-card h3 {
            font-size: 1.5rem;
            color: var(--text-primary);
            margin-bottom: 15px;
            text-align: center;
            position: relative;
        }
        
        .service-price {
            font-size: 1.8rem;
            font-weight: bold;
            color: var(--primary);
            text-align: center;
            margin-bottom: 20px;
            position: relative;
        }
        
        .service-features {
            list-style: none;
            padding: 0;
            margin-bottom: 30px;
            position: relative;
        }
        
        .service-features li {
            padding: 12px 0;
            color: var(--text-secondary);
            display: flex;
            align-items: center;
            border-bottom: 1px solid #2a2a2a;
        }
        
        .service-features li:last-child {
            border-bottom: none;
        }
        
        .service-features i {
            margin-right: 12px;
            color: var(--primary);
            font-size: 1.1rem;
        }
        
        /* Button Styles */
        .btn {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            background: var(--primary);
            color: white;
            padding: 14px 28px;
            border-radius: 8px;
            text-decoration: none;
            font-weight: 600;
            transition: all 0.3s ease;
            width: 100%;
            border: none;
            cursor: pointer;
            position: relative;
            overflow: hidden;
            z-index: 1;
            box-shadow: 0 4px 15px rgba(58, 168, 255, 0.3);
        }
        
        .btn span {
            position: relative;
            z-index: 2;
        }
        
        .btn i {
            margin-left: 10px;
            font-size: 1.2rem;
            position: relative;
            z-index: 2;
        }
        
        .btn::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.2), transparent);
            transition: 0.5s;
            z-index: 1;
        }
        
        .btn:hover {
            background: var(--primary-dark);
            transform: translateY(-3px);
            box-shadow: 0 8px 25px rgba(58, 168, 255, 0.4);
        }
        
        .btn:hover::before {
            left: 100%;
        }
        
        /* Glow Effect on Hover */
        .service-card:hover .service-icon {
            animation: glow 1.5s ease-in-out infinite alternate;
        }
        
        @keyframes glow {
            from {
                text-shadow: 0 0 5px rgba(58, 168, 255, 0.5);
            }
            to {
                text-shadow: 0 0 15px rgba(58, 168, 255, 0.8);
            }
        }
        
        /* Responsive Adjustments */
        @media (max-width: 768px) {
            .service-grid {
                grid-template-columns: 1fr;
            }
            
            .services {
                padding: 50px 0;
            }
            
            .service-card {
                padding: 25px;
            }
        }
    </style>
</head>
<body>
    <!-- Services Section -->
    <section class="services" id="services">
        <div class="container">
            <h2>Paket Layanan Kami</h2>
            <p class="section-subtitle">Solusi lengkap untuk masalah kaki-kaki mobil Anda</p>
            
            <div class="service-grid">
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-car-steering"></i>
                    </div>
                    <h3>Paket Racksteer</h3>
                    <div class="service-price">Rp 1.200.000</div>
                    <ul class="service-features">
                        <li><i class="fas fa-check-circle"></i> Perbaikan sistem racksteer</li>
                        <li><i class="fas fa-check-circle"></i> Ganti sparepart yang rusak</li>
                        <li><i class="fas fa-check-circle"></i> Penyetelan ulang</li>
                        <li><i class="fas fa-check-circle"></i> Garansi 1 tahun</li>
                    </ul>
                    <a href="https://wa.me/6281226298787" class="btn" target="_blank">
                        <span>Pesan Sekarang</span>
                        <i class="fab fa-whatsapp"></i>
                    </a>
                </div>
                
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-car-crash"></i>
                    </div>
                    <h3>Paket Shockbreaker</h3>
                    <div class="service-price">Rp 1.200.000</div>
                    <ul class="service-features">
                        <li><i class="fas fa-check-circle"></i> Perbaikan shockbreaker</li>
                        <li><i class="fas fa-check-circle"></i> Ganti sparepart yang rusak</li>
                        <li><i class="fas fa-check-circle"></i> Penyetelan ulang</li>
                        <li><i class="fas fa-check-circle"></i> Garansi 1 tahun</li>
                    </ul>
                    <a href="https://wa.me/6281226298787" class="btn" target="_blank">
                        <span>Pesan Sekarang</span>
                        <i class="fab fa-whatsapp"></i>
                    </a>
                </div>
                
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-cogs"></i>
                    </div>
                    <h3>Paket Perawatan Rutin</h3>
                    <div class="service-price">Rp 800.000</div>
                    <ul class="service-features">
                        <li><i class="fas fa-check-circle"></i> Pemeriksaan komprehensif</li>
                        <li><i class="fas fa-check-circle"></i> Pelumasan komponen</li>
                        <li><i class="fas fa-check-circle"></i> Penyetelan ulang</li>
                        <li><i class="fas fa-check-circle"></i> Garansi 6 bulan</li>
                    </ul>
                    <a href="https://wa.me/6281226298787" class="btn" target="_blank">
                        <span>Pesan Sekarang</span>
                        <i class="fab fa-whatsapp"></i>
                    </a>
                </div>
            </div>
        </div>
    </section>
</body>
</html>
    <!-- Locations Section -->
    <section class="locations" id="locations">
        <div class="container">
            <h2 class="section-title">Cabang Kami</h2>
            <p class="section-subtitle">Temukan bengkel Prast Kaki Kaki terdekat</p>
            
            <div class="location-cards">
                <!-- Cabang 1 -->
                <div class="location-card">
                    <span class="location-badge">Buka 24 Jam</span>
                    <h3>Jakarta Pusat</h3>
                    
                    <div class="location-details">
                        <div class="location-detail">
                            <i class="fas fa-map-marker-alt"></i>
                            <span>Jl. Cikini Raya No. 73, Jakarta Pusat 10330</span>
                        </div>
                        
                        <div class="location-detail">
                            <i class="fas fa-clock"></i>
                            <span>Senin - Minggu: 08:00 - 22:00 WIB<small>Layanan darurat 24 jam</small></span>
                        </div>
                        
                        <div class="location-detail">
                            <i class="fas fa-phone-alt"></i>
                            <span>(021) 1234-5678 / 0812-3456-7890</span>
                        </div>
                        
                        <div class="location-detail">
                            <i class="fas fa-star"></i>
                            <span>Fasilitas lengkap • Parkir luas • Coffee shop</span>
                        </div>
                    </div>
                    
                    <div class="location-actions">
                        <a href="https://maps.google.com/?q=Jl.+Cikini+Raya+No.+73+Jakarta" class="location-btn" target="_blank">
                            Lihat Peta <i class="fas fa-map-marked-alt"></i>
                        </a>
                        <a href="tel:+622112345678" class="location-btn primary">
                            Telepon <i class="fas fa-phone"></i>
                        </a>
                    </div>
                </div>
                
                <!-- Cabang 2 -->
                <div class="location-card">
                    <h3>Depok</h3>
                    
                    <div class="location-details">
                        <div class="location-detail">
                            <i class="fas fa-map-marker-alt"></i>
                            <span>Jl. Margonda Raya No. 256, Depok 16424</span>
                        </div>
                        
                        <div class="location-detail">
                            <i class="fas fa-clock"></i>
                            <span>Senin - Minggu: 08:00 - 20:00 WIB</span>
                        </div>
                        
                        <div class="location-detail">
                            <i class="fas fa-phone-alt"></i>
                            <span>(021) 8765-4321 / 0813-4567-8901</span>
                        </div>
                        
                        <div class="location-detail">
                            <i class="fas fa-star"></i>
                            <span>Area tunggu nyaman • Free WiFi • Toilet bersih</span>
                        </div>
                    </div>
                    
                    <div class="location-actions">
                        <a href="https://maps.google.com/?q=Jl.+Margonda+Raya+No.+256+Depok" class="location-btn" target="_blank">
                            Lihat Peta <i class="fas fa-map-marked-alt"></i>
                        </a>
                        <a href="tel:+622187654321" class="location-btn primary">
                            Telepon <i class="fas fa-phone"></i>
                        </a>
                    </div>
                </div>
                
                <!-- Cabang 3 -->
                <div class="location-card">
                    <span class="location-badge">Promo Spesial</span>
                    <h3>Tangerang</h3>
                    
                    <div class="location-details">
                        <div class="location-detail">
                            <i class="fas fa-map-marker-alt"></i>
                            <span>Jl. Jend. Sudirman No. 45, Tangerang 15111</span>
                        </div>
                        
                        <div class="location-detail">
                            <i class="fas fa-clock"></i>
                            <span>Senin - Minggu: 08:00 - 20:00 WIB</span>
                        </div>
                        
                        <div class="location-detail">
                            <i class="fas fa-phone-alt"></i>
                            <span>(021) 9876-5432 / 0812-7654-3210</span>
                        </div>
                        
                        <div class="location-detail">
                            <i class="fas fa-star"></i>
                            <span>Area kids friendly • Free car wash • Vending machine</span>
                        </div>
                    </div>
                    
                    <div class="location-actions">
                        <a href="https://maps.google.com/?q=Jl.+Jend.+Sudirman+No.+45+Tangerang" class="location-btn" target="_blank">
                            Lihat Peta <i class="fas fa-map-marked-alt"></i>
                        </a>
                        <a href="tel:+622198765432" class="location-btn primary">
                            Telepon <i class="fas fa-phone"></i>
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </section>
</body>
</html>
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>PRAST KAKI KAKI - Kontak Kami</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        /* ==== GLOBAL VARIABLES ==== */
        :root {
            --primary: #0066ff;
            --primary-light: rgba(0, 102, 255, 0.1);
            --secondary: #e0e0e0;
            --dark: #0a0a0a;
            --darker: #050505;
            --accent: #00ffcc;
            --accent-dark: #00cca3;
            --text: #ffffff;
            --text-muted: #aaaaaa;
            --card-bg: rgba(30, 30, 30, 0.8);
            --whatsapp: #25D366;
            --facebook: #1877F2;
            --instagram: #E4405F;
            --tiktok: #000000;
        }

        /* ==== CONTACT SECTION ==== */
        .contact {
            padding: 6rem 0;
            text-align: center;
            background: linear-gradient(135deg, var(--darker), var(--dark));
            position: relative;
            overflow: hidden;
        }

        .contact::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: radial-gradient(circle at 80% 20%, rgba(0,255,204,0.05) 0%, transparent 50%);
            z-index: 0;
        }

        .contact .container {
            position: relative;
            z-index: 1;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 2rem;
        }

        .section-title {
            font-size: 2.8rem;
            font-weight: 700;
            margin-bottom: 1rem;
            background: linear-gradient(90deg, var(--primary), var(--accent));
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            display: inline-block;
        }

        .section-subtitle {
            color: var(--text-muted);
            font-size: 1.2rem;
            margin-bottom: 3rem;
            position: relative;
            display: inline-block;
        }

        .section-subtitle::after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
            width: 60px;
            height: 3px;
            background: linear-gradient(90deg, var(--primary), var(--accent));
        }

        .contact-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin-top: 3rem;
        }

        .contact-card {
            background: var(--card-bg);
            padding: 2.5rem;
            border-radius: 12px;
            transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.1);
            border: 1px solid rgba(0, 102, 255, 0.2);
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
            backdrop-filter: blur(5px);
            position: relative;
            overflow: hidden;
        }

        .contact-card::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 100%;
            height: 4px;
            background: linear-gradient(90deg, var(--primary), var(--accent));
            transition: all 0.3s;
        }

        .contact-card:hover {
            transform: translateY(-8px);
            box-shadow: 0 15px 40px rgba(0, 102, 255, 0.3);
        }

        .contact-card:hover::after {
            height: 8px;
        }

        .contact-icon {
            font-size: 2.5rem;
            margin-bottom: 1.5rem;
            display: inline-block;
            transition: all 0.3s;
        }

        .contact-card:hover .contact-icon {
            transform: scale(1.1) translateY(-5px);
        }

        .contact-card h3 {
            color: var(--primary);
            font-size: 1.8rem;
            margin-bottom: 1.5rem;
            font-weight: 600;
        }

        .contact-info {
            color: var(--secondary);
            margin-bottom: 2rem;
            line-height: 1.7;
        }

        .social-links {
            display: flex;
            justify-content: center;
            gap: 1.5rem;
            margin-top: 2rem;
            flex-wrap: wrap;
        }

        .social-link {
            display: flex;
            align-items: center;
            justify-content: center;
            width: 60px;
            height: 60px;
            border-radius: 50%;
            font-size: 1.8rem;
            color: white;
            transition: all 0.3s cubic-bezier(0.175, 0.885, 0.32, 1.275);
            position: relative;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0,0,0,0.2);
        }

        .social-link::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(135deg, rgba(255,255,255,0.3), transparent);
            transform: translateY(-100%);
            transition: all 0.3s;
        }

        .social-link:hover {
            transform: translateY(-5px) scale(1.1);
            box-shadow: 0 10px 20px rgba(0,0,0,0.3);
        }

        .social-link:hover::before {
            transform: translateY(0);
        }

        .whatsapp { background-color: var(--whatsapp); }
        .facebook { background-color: var(--facebook); }
        .instagram { 
            background: radial-gradient(circle at 30% 107%, #fdf497 0%, #fdf497 5%, #fd5949 45%, #d6249f 60%, #285AEB 90%);
        }
        .tiktok { background-color: var(--tiktok); }

        .contact-form {
            max-width: 600px;
            margin: 0 auto;
            padding: 2rem;
            background: var(--card-bg);
            border-radius: 12px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.2);
            backdrop-filter: blur(5px);
            border: 1px solid rgba(0,102,255,0.2);
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .contact {
                padding: 4rem 0;
            }
            
            .section-title {
                font-size: 2.2rem;
            }
            
            .section-subtitle {
                font-size: 1rem;
            }
            
            .contact-grid {
                grid-template-columns: 1fr;
            }
            
            .social-link {
                width: 50px;
                height: 50px;
                font-size: 1.5rem;
            }
        }
    </style>
</head>
<body>
<!-- Contact Section -->
<section class="contact" id="contact">
    <div class="container">
        <h2 class="section-title">Hubungi Kami</h2>
        <p class="section-subtitle">Tetap terhubung dengan Prast Kaki Kaki</p>
        
        <div class="contact-grid">
            <!-- Phone Card -->
            <div class="contact-card">
                <div class="contact-icon">
                    <i class="fas fa-phone-alt"></i>
                </div>
                <div class="contact-content">
                    <h3>Telepon</h3>
                    <div class="contact-info">
                        <a href="tel:+622112345678" class="contact-link">
                            <i class="fas fa-phone"></i> (021) 1234-5678
                        </a>
                        <a href="tel:+6281234567890" class="contact-link">
                            <i class="fas fa-mobile-alt"></i> 0812-3456-7890
                        </a>
                    </div>
                </div>
            </div>
            
            <!-- Email Card -->
            <div class="contact-card">
                <div class="contact-icon">
                    <i class="fas fa-envelope"></i>
                </div>
                <div class="contact-content">
                    <h3>Email</h3>
                    <div class="contact-info">
                        <a href="mailto:bengkelprastkakikaki@gmail.com?subject=Konsultasi%20Layanan&body=Halo%20Bengkel%20Prast,%0A%0ASaya%20ingin%20konsultasi%20tentang..." class="contact-link email-link">
                            <i class="fas fa-envelope-open-text"></i> bengkelprastkakikaki@gmail.com
                        </a>
                        <a href="mailto:prastkakikakicabangsolo@gmail.com?subject=Konsultasi%20Layanan&body=Halo%20Bengkel%20Prast,%0A%0ASaya%20ingin%20konsultasi%20tentang..." class="contact-link email-link">
                            <i class="fas fa-envelope"></i> prastkakikakicabangsolo@gmail.com
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </div>
</section>

<style>
    /* Automotive Dark Blue Theme */
    :root {
        --primary: #2563eb;       /* Rich blue */
        --primary-dark: #1e40af;  /* Darker blue */
        --dark-bg: #0f172a;       /* Deep navy */
        --dark-card: #1e293b;     /* Slightly lighter navy */
        --text-primary: #e2e8f0;  /* Light blue-gray */
        --text-secondary: #94a3b8;/* Medium blue-gray */
        --accent: #60a5fa;        /* Bright blue accent */
    }
    
    .contact {
        background-color: var(--dark-bg);
        padding: 80px 0;
        font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    }
    
    .container {
        max-width: 1200px;
        margin: 0 auto;
        padding: 0 20px;
    }
    
    .section-title {
        text-align: center;
        font-size: 2.5rem;
        color: var(--text-primary);
        margin-bottom: 15px;
        position: relative;
    }
    
    .section-title::after {
        content: '';
        display: block;
        width: 80px;
        height: 4px;
        background: var(--primary);
        margin: 15px auto;
        border-radius: 2px;
    }
    
    .section-subtitle {
        text-align: center;
        color: var(--text-secondary);
        font-size: 1.1rem;
        margin-bottom: 50px;
    }
    
    .contact-grid {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
        gap: 30px;
        margin-top: 40px;
    }
    
    .contact-card {
        background: var(--dark-card);
        border-radius: 12px;
        padding: 30px;
        display: flex;
        align-items: flex-start;
        gap: 20px;
        border: 1px solid #334155;
        transition: all 0.3s ease;
        box-shadow: 0 5px 20px rgba(0, 0, 0, 0.3);
        position: relative;
        overflow: hidden;
    }
    
    .contact-card::before {
        content: '';
        position: absolute;
        bottom: 0;
        left: 0;
        width: 100%;
        height: 3px;
        background: var(--primary);
        transform: scaleX(0);
        transform-origin: left;
        transition: transform 0.3s ease;
    }
    
    .contact-card:hover {
        transform: translateY(-5px);
        box-shadow: 0 15px 30px rgba(37, 99, 235, 0.2);
        border-color: var(--primary);
    }
    
    .contact-card:hover::before {
        transform: scaleX(1);
    }
    
    .contact-icon {
        font-size: 2rem;
        color: var(--accent);
        background: rgba(37, 99, 235, 0.1);
        width: 60px;
        height: 60px;
        border-radius: 50%;
        display: flex;
        align-items: center;
        justify-content: center;
        flex-shrink: 0;
        transition: all 0.3s ease;
    }
    
    .contact-card:hover .contact-icon {
        background: rgba(37, 99, 235, 0.2);
        transform: rotate(15deg);
    }
    
    .contact-content {
        flex: 1;
    }
    
    .contact-card h3 {
        color: var(--text-primary);
        font-size: 1.4rem;
        margin-bottom: 15px;
        font-weight: 600;
    }
    
    .contact-info {
        display: flex;
        flex-direction: column;
        gap: 12px;
    }
    
    .contact-link {
        color: var(--text-secondary);
        text-decoration: none;
        transition: all 0.3s ease;
        display: flex;
        align-items: center;
        gap: 10px;
        padding: 10px 15px;
        border-radius: 8px;
        background: rgba(30, 41, 59, 0.5);
        border: 1px solid #334155;
    }
    
    .contact-link i {
        color: var(--accent);
        font-size: 1.1rem;
        transition: all 0.3s ease;
    }
    
    .contact-link:hover {
        color: var(--text-primary);
        background: rgba(37, 99, 235, 0.1);
        border-color: var(--primary);
        transform: translateX(5px);
    }
    
    .contact-link:hover i {
        color: var(--primary);
        transform: scale(1.1);
    }
    
    .email-link::after {
        content: " ↗";
        font-size: 0.85em;
        margin-left: auto;
        opacity: 0.7;
        transition: all 0.3s ease;
    }
    
    .email-link:hover::after {
        opacity: 1;
        transform: translateX(3px);
    }
    
    /* Responsive Design */
    @media (max-width: 768px) {
        .contact-grid {
            grid-template-columns: 1fr;
        }
        
        .contact-card {
            flex-direction: column;
            align-items: center;
            text-align: center;
            padding: 25px;
        }
        
        .contact-info {
            align-items: center;
        }
        
        .contact-link {
            flex-direction: column;
            text-align: center;
            gap: 5px;
        }
        
        .email-link::after {
            display: none;
        }
    }
</style>
<!-- Footer Section -->
<footer class="footer" id="footer">
    <div class="container">
        <div class="footer-grid">
            <!-- Company Profile Column -->
            <div class="footer-profile">
                <div class="cyber-header">
                    <h3 class="footer-title glitch" data-text="Prast Kaki Kaki">Prast Kaki Kaki</h3>
                    <div class="cyber-line"></div>
                </div>
                
                <p class="footer-description neon-text">
                    <span class="flicker">Spesialis perbaikan sistem kemudi & suspensi mobil sejak 2015</span><br>
                    <span class="fast-flicker">8.500+ mobil telah diperbaiki</span>
                </p>
                
                <div class="guarantee-badges">
                    <div class="guarantee-badge cyber-badge">
                        <i class="fas fa-shield-alt"></i> Garansi Kepuasan
                        <div class="cyber-dots"></div>
                    </div>
                    <div class="guarantee-badge cyber-badge">
                        <i class="fas fa-sync-alt"></i> Free Cek Komponen
                        <div class="cyber-dots"></div>
                    </div>
                </div>
                
                <div class="footer-contacts">
                    <div class="contact-item cyber-contact">
                        <i class="fas fa-map-marker-alt pulse"></i>
                        <div>
                            <h4>Pusat</h4>
                            <p>Jl. Kedungmundu No.168 A, Semarang</p>
                        </div>
                    </div>
                    <div class="contact-item cyber-contact">
                        <i class="fas fa-store pulse"></i>
                        <div>
                            <h4>Cabang</h4>
                            <p>Jl. Samratulangi No.44B, Manahan, Solo</p>
                        </div>
                    </div>
                </div>
            </div>
            
            <!-- Booking Form Column -->
            <div class="footer-form cyber-form">
                <div class="cyber-header">
                    <h3 class="footer-title glitch" data-text="Booking Cek Gratis">Booking Cek Gratis</h3>
                    <div class="cyber-line"></div>
                </div>
                
                <form id="bookingForm" class="message-form">
                    <div class="form-group cyber-input">
                        <label for="cabang">Pilih Cabang</label>
                        <select id="cabang" name="cabang" required>
                            <option value="" disabled selected>-- Pilih Cabang --</option>
                            <option value="Semarang">Semarang (Jl. Kedungmundu No.168 A)</option>
                            <option value="Solo">Solo (Jl. Samratulangi No.44B)</option>
                        </select>
                        <div class="cyber-underline"></div>
                    </div>
                    
                    <div class="form-group">
                        <label>Pilih Waktu</label>
                        <div class="time-options">
                            <label class="time-option cyber-radio">
                                <input type="radio" name="waktu" value="Pagi (08:00 - 11:00)" required>
                                <span class="cyber-radio-btn"></span>
                                <span class="cyber-radio-text">Pagi (08:00-11:00)</span>
                            </label>
                            <label class="time-option cyber-radio">
                                <input type="radio" name="waktu" value="Siang (13:00 - 16:00)">
                                <span class="cyber-radio-btn"></span>
                                <span class="cyber-radio-text">Siang (13:00-16:00)</span>
                            </label>
                        </div>
                    </div>
                    
                    <div class="form-group cyber-input">
                        <label for="nama">Nama Lengkap</label>
                        <input type="text" id="nama" name="nama" placeholder="Budi Santoso" required>
                        <div class="cyber-underline"></div>
                    </div>
                    
                    <div class="form-group cyber-input">
                        <label for="mobil">Jenis Mobil</label>
                        <input type="text" id="mobil" name="mobil" placeholder="Toyota Avanza" required>
                        <div class="cyber-underline"></div>
                    </div>
                    
                    <div class="form-group cyber-input">
                        <label for="plat">Nomor Plat</label>
                        <input type="text" id="plat" name="plat" placeholder="H 1234 ABC" required>
                        <div class="cyber-underline"></div>
                    </div>
                    
                    <div class="form-group cyber-input">
                        <label for="whatsapp">Nomor WhatsApp</label>
                        <input type="tel" id="whatsapp" name="whatsapp" placeholder="08123456789" required>
                        <div class="cyber-underline"></div>
                    </div>
                    
                    <button type="submit" class="submit-btn cyber-btn">
                        <i class="fab fa-whatsapp"></i> 
                        <span class="btn-text">Booking via WhatsApp</span>
                        <span class="cyber-glow"></span>
                    </button>
                </form>
            </div>
            
            <!-- Services Column -->
            <div class="footer-links cyber-links">
                <div class="cyber-header">
                    <h3 class="footer-title glitch" data-text="Layanan Kami">Layanan Kami</h3>
                    <div class="cyber-line"></div>
                </div>
                
                <ul class="services-list cyber-list">
                    <li><a href="#services"><span class="link-hover">Perbaikan Racksteer</span></a></li>
                    <li><a href="#services"><span class="link-hover">Ganti Shockbreaker</span></a></li>
                    <li><a href="#services"><span class="link-hover">Spooring & Balancing</span></a></li>
                    <li><a href="#services"><span class="link-hover">Perawatan Rutin</span></a></li>
                </ul>
                
                <div class="guarantee-notes cyber-notes">
                    <p><i class="fas fa-check-circle pulse"></i> <span class="neon-text">Jika rusak selama garansi, kami bongkar ulang GRATIS</span></p>
                    <p><i class="fas fa-check-circle pulse"></i> <span class="neon-text">Ganti sparepart baru + uang kembali jika tidak puas</span></p>
                </div>
                
                <a href="https://wa.me/6281226298787" class="footer-cta cyber-cta">
                    <i class="fab fa-whatsapp"></i> 
                    <span>Konsultasi Gratis</span>
                    <div class="cyber-dots"></div>
                </a>
            </div>
        </div>
        
        <!-- Footer Bottom -->
        <div class="footer-bottom cyber-footer">
            <div class="scanline"></div>
            <p class="cyber-copyright">© <span class="year"></span> Prast Kaki Kaki. All Systems Operational.</p>
        </div>
    </div>
</footer>

<style>
    /* ===== Cyberpunk Base Styles ===== */
    :root {
        --neon-blue: #3aa8ff;
        --neon-pink: #ff2a6d;
        --neon-green: #05f0ff;
        --dark-bg: #0a0a12;
        --darker-bg: #06060a;
        --cyber-text: #e2e8f0;
        --cyber-accent: #00f7ff;
    }
    
    @font-face {
        font-family: 'Cyber';
        src: url('https://fonts.cdnfonts.com/css/cyberpunk-is-not-dead');
    }
    
    /* ===== Animation Keyframes ===== */
    @keyframes flicker {
        0%, 19%, 21%, 23%, 25%, 54%, 56%, 100% { opacity: 1; }
        20%, 22%, 24%, 55% { opacity: 0.4; }
    }
    
    @keyframes fastFlicker {
        0%, 10%, 12%, 14%, 16%, 18%, 20%, 100% { opacity: 1; }
        11%, 13%, 15%, 17%, 19% { opacity: 0.3; }
    }
    
    @keyframes pulse {
        0%, 100% { opacity: 1; }
        50% { opacity: 0.6; }
    }
    
    @keyframes glitch {
        0% { text-shadow: 0.05em 0 0 var(--neon-blue), -0.05em -0.025em 0 var(--neon-pink); }
        14% { text-shadow: 0.05em 0 0 var(--neon-blue), -0.05em -0.025em 0 var(--neon-pink); }
        15% { text-shadow: -0.05em -0.025em 0 var(--neon-blue), 0.025em 0.025em 0 var(--neon-pink); }
        49% { text-shadow: -0.05em -0.025em 0 var(--neon-blue), 0.025em 0.025em 0 var(--neon-pink); }
        50% { text-shadow: 0.025em 0.05em 0 var(--neon-blue), 0.05em 0 0 var(--neon-pink); }
        99% { text-shadow: 0.025em 0.05em 0 var(--neon-blue), 0.05em 0 0 var(--neon-pink); }
        100% { text-shadow: -0.025em 0 0 var(--neon-blue), -0.025em -0.025em 0 var(--neon-pink); }
    }
    
    @keyframes scanline {
        0% { transform: translateY(0); }
        100% { transform: translateY(100%); }
    }
    
    /* ===== Core Footer Styles ===== */
    .footer {
        background: var(--dark-bg);
        color: var(--cyber-text);
        padding: 60px 0 0;
        font-family: 'Segoe UI', sans-serif;
        position: relative;
        overflow: hidden;
        border-top: 1px solid var(--neon-blue);
    }
    
    .footer::before {
        content: '';
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background: 
            linear-gradient(90deg, 
                transparent 0%, 
                rgba(58, 168, 255, 0.05) 50%, 
                transparent 100%);
        pointer-events: none;
    }
    
    .container {
        max-width: 1200px;
        margin: 0 auto;
        padding: 0 20px;
        position: relative;
        z-index: 1;
    }
    
    .footer-grid {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
        gap: 40px;
        margin-bottom: 40px;
    }
    
    /* ===== Cyberpunk Elements ===== */
    .cyber-header {
        margin-bottom: 25px;
        position: relative;
    }
    
    .cyber-line {
        height: 2px;
        background: linear-gradient(90deg, var(--neon-blue), transparent);
        margin-top: 10px;
    }
    
    .glitch {
        position: relative;
        font-family: 'Cyber', sans-serif;
        font-weight: 700;
        animation: glitch 2000ms infinite;
    }
    
    .glitch::before {
        content: attr(data-text);
        position: absolute;
        left: 0;
        text-shadow: -2px 0 var(--neon-pink);
        clip: rect(0, 900px, 0, 0);
        animation: glitch 3s infinite alternate-reverse;
    }
    
    .neon-text {
        text-shadow: 0 0 5px var(--neon-blue);
    }
    
    .flicker {
        animation: flicker 3s infinite alternate;
    }
    
    .fast-flicker {
        animation: fastFlicker 1.5s infinite alternate;
    }
    
    .pulse {
        animation: pulse 2s infinite;
    }
    
    /* ===== Profile Section ===== */
    .footer-profile {
        display: flex;
        flex-direction: column;
    }
    
    .footer-title {
        font-size: 1.8rem;
        color: var(--neon-blue);
        margin-bottom: 15px;
        letter-spacing: 1px;
    }
    
    .footer-description {
        line-height: 1.6;
        color: #94a3b8;
        margin: 15px 0;
        font-size: 1rem;
    }
    
    /* Guarantee Badges */
    .guarantee-badges {
        display: flex;
        flex-wrap: wrap;
        gap: 10px;
        margin: 20px 0;
    }
    
    .cyber-badge {
        background: rgba(58, 168, 255, 0.1);
        border: 1px solid var(--neon-blue);
        color: var(--neon-blue);
        padding: 10px 15px;
        border-radius: 0;
        font-size: 0.85rem;
        display: flex;
        align-items: center;
        gap: 10px;
        position: relative;
        overflow: hidden;
    }
    
    .cyber-badge:hover {
        background: rgba(58, 168, 255, 0.2);
        box-shadow: 0 0 10px var(--neon-blue);
    }
    
    .cyber-dots {
        position: absolute;
        right: 10px;
        display: flex;
        gap: 3px;
    }
    
    .cyber-dots::before {
        content: '•••';
        color: var(--neon-blue);
        font-size: 0.6rem;
        letter-spacing: 1px;
    }
    
    /* Contact Info */
    .footer-contacts {
        margin: 25px 0;
    }
    
    .cyber-contact {
        display: flex;
        gap: 15px;
        align-items: flex-start;
        margin-bottom: 15px;
        padding: 10px;
        transition: all 0.3s;
        position: relative;
    }
    
    .cyber-contact:hover {
        background: rgba(58, 168, 255, 0.05);
    }
    
    .cyber-contact::before {
        content: '';
        position: absolute;
        left: 0;
        bottom: 0;
        width: 100%;
        height: 1px;
        background: linear-gradient(90deg, var(--neon-blue), transparent);
    }
    
    .cyber-contact i {
        color: var(--neon-blue);
        font-size: 1.2rem;
    }
    
    .cyber-contact h4 {
        color: var(--cyber-text);
        margin-bottom: 5px;
        font-size: 1rem;
        text-transform: uppercase;
        letter-spacing: 1px;
    }
    
    .cyber-contact p {
        color: #94a3b8;
        margin: 0;
        font-size: 0.9rem;
    }
    
    /* ===== Booking Form ===== */
    .cyber-form {
        background: rgba(10, 10, 18, 0.7);
        border: 1px solid var(--neon-blue);
        padding: 25px;
        box-shadow: 0 0 20px rgba(58, 168, 255, 0.1);
        position: relative;
    }
    
    .cyber-form::before {
        content: '';
        position: absolute;
        top: 0;
        left: 0;
        right: 0;
        height: 1px;
        background: linear-gradient(90deg, transparent, var(--neon-blue), transparent);
    }
    
    .message-form {
        display: grid;
        gap: 20px;
    }
    
    .cyber-input {
        position: relative;
    }
    
    .cyber-input label {
        display: block;
        color: var(--neon-blue);
        margin-bottom: 8px;
        font-size: 0.9rem;
        text-transform: uppercase;
        letter-spacing: 1px;
    }
    
    .cyber-input input,
    .cyber-input select {
        width: 100%;
        padding: 12px 0;
        background: transparent;
        border: none;
        border-bottom: 1px solid #334155;
        color: white;
        font-family: inherit;
        font-size: 1rem;
    }
    
    .cyber-input input:focus,
    .cyber-input select:focus {
        outline: none;
    }
    
    .cyber-underline {
        position: absolute;
        bottom: 0;
        left: 0;
        width: 0;
        height: 2px;
        background: var(--neon-blue);
        transition: width 0.3s;
    }
    
    .cyber-input input:focus ~ .cyber-underline,
    .cyber-input select:focus ~ .cyber-underline {
        width: 100%;
    }
    
    /* Time Selection */
    .time-options {
        display: flex;
        gap: 15px;
        margin-top: 10px;
    }
    
    .cyber-radio {
        display: flex;
        align-items: center;
        gap: 10px;
        cursor: pointer;
        position: relative;
    }
    
    .cyber-radio input {
        position: absolute;
        opacity: 0;
    }
    
    .cyber-radio-btn {
        width: 18px;
        height: 18px;
        border: 2px solid var(--neon-blue);
        position: relative;
    }
    
    .cyber-radio-btn::before {
        content: '';
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        width: 10px;
        height: 10px;
        background: var(--neon-blue);
        opacity: 0;
        transition: opacity 0.3s;
    }
    
    .cyber-radio input:checked ~ .cyber-radio-btn::before {
        opacity: 1;
    }
    
    .cyber-radio-text {
        color: #94a3b8;
        transition: color 0.3s;
    }
    
    .cyber-radio input:checked ~ .cyber-radio-text {
        color: var(--neon-blue);
    }
    
    /* Submit Button */
    .cyber-btn {
        background: transparent;
        color: var(--neon-green);
        border: 1px solid var(--neon-green);
        padding: 15px;
        font-weight: bold;
        text-transform: uppercase;
        letter-spacing: 1px;
        position: relative;
        overflow: hidden;
        display: flex;
        align-items: center;
        justify-content: center;
        gap: 10px;
        margin-top: 20px;
        transition: all 0.3s;
    }
    
    .cyber-btn:hover {
        background: rgba(5, 240, 255, 0.1);
        box-shadow: 0 0 15px var(--neon-green);
    }
    
    .cyber-glow {
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background: linear-gradient(90deg, 
            transparent 0%, 
            rgba(5, 240, 255, 0.3) 50%, 
            transparent 100%);
        opacity: 0;
        transition: opacity 0.3s;
    }
    
    .cyber-btn:hover .cyber-glow {
        opacity: 1;
    }
    
    /* ===== Services Section ===== */
    .cyber-links {
        display: flex;
        flex-direction: column;
    }
    
    .cyber-list {
        list-style: none;
        padding: 0;
        margin: 20px 0;
    }
    
    .cyber-list li {
        margin-bottom: 15px;
        position: relative;
    }
    
    .cyber-list li::before {
        content: '>';
        color: var(--neon-blue);
        margin-right: 10px;
    }
    
    .link-hover {
        color: #94a3b8;
        position: relative;
        transition: color 0.3s;
    }
    
    .link-hover::after {
        content: '';
        position: absolute;
        bottom: -2px;
        left: 0;
        width: 0;
        height: 1px;
        background: var(--neon-blue);
        transition: width 0.3s;
    }
    
    .cyber-list a:hover .link-hover {
        color: var(--neon-blue);
    }
    
    .cyber-list a:hover .link-hover::after {
        width: 100%;
    }
    
    /* Guarantee Notes */
    .cyber-notes {
        background: rgba(58, 168, 255, 0.05);
        border-left: 3px solid var(--neon-blue);
        padding: 15px;
        margin-top: 25px;
    }
    
    .cyber-notes p {
        color: #94a3b8;
        font-size: 0.85rem;
        margin-bottom: 10px;
        display: flex;
        align-items: flex-start;
        gap: 10px;
    }
    
    .cyber-notes i {
        color: var(--neon-blue);
    }
    
    /* CTA Button */
    .cyber-cta {
        background: rgba(58, 168, 255, 0.1);
        color: var(--neon-blue);
        padding: 12px 20px;
        text-decoration: none;
        display: flex;
        align-items: center;
        gap: 10px;
        margin-top: 20px;
        position: relative;
        overflow: hidden;
        border: 1px solid var(--neon-blue);
        transition: all 0.3s;
    }
    
    .cyber-cta:hover {
        background: rgba(58, 168, 255, 0.2);
        box-shadow: 0 0 15px var(--neon-blue);
    }
    
    /* ===== Footer Bottom ===== */
    .cyber-footer {
        border-top: 1px solid var(--neon-blue);
        padding: 20px 0;
        position: relative;
        overflow: hidden;
    }
    
    .scanline {
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 1px;
        background: linear-gradient(90deg, transparent, var(--neon-blue), transparent);
        animation: scanline 6s linear infinite;
    }
    
    .cyber-copyright {
        color: #64748b;
        font-size: 0.8rem;
        text-align: center;
        text-transform: uppercase;
        letter-spacing: 1px;
    }
    
    /* ===== Responsive Design ===== */
    @media (max-width: 768px) {
        .footer-grid {
            grid-template-columns: 1fr;
            gap: 30px;
        }
        
        .footer {
            padding: 40px 0 0;
        }
        
        .time-options {
            flex-direction: column;
        }
        
        .footer-title {
            font-size: 1.5rem;
        }
    }
</style>

<script>
    // Auto-update copyright year
    document.querySelector('.year').textContent = new Date().getFullYear();
    
    // Booking form handler
    document.getElementById('bookingForm').addEventListener('submit', function(e) {
        e.preventDefault();
        
        const formData = new FormData(this);
        const data = Object.fromEntries(formData);
        
        const message = `*BOOKING CEK GRATIS*%0A%0A` +
                        `*Nama*: ${data.nama}%0A` +
                        `*Cabang*: ${data.cabang}%0A` +
                        `*Waktu*: ${data.waktu}%0A` +
                        `*Mobil*: ${data.mobil}%0A` +
                        `*Plat*: ${data.plat}%0A%0A` +
                        `*Nomor WhatsApp*: ${data.whatsapp}%0A%0A` +
                        `_Mohon konfirmasi ketersediaan jadwalnya. Terima kasih._`;
        
        window.open(`https://wa.me/6281226298787?text=${message}`, '_blank');
    });
    
    // Add hover effect to inputs
    const inputs = document.querySelectorAll('.cyber-input input, .cyber-input select');
    inputs.forEach(input => {
        input.addEventListener('focus', function() {
            this.parentElement.querySelector('.cyber-underline').style.width = '100%';
        });
        
        input.addEventListener('blur', function() {
            if (!this.value) {
                this.parentElement.querySelector('.cyber-underline').style.width = '0';
            }
        });
    });
</script>
        
        <!-- Social & Copyright -->
        <div class="footer-bottom">
            <div class="social-links">
                <a href="https://wa.me/6281226298787" class="social-link whatsapp" target="_blank">
                    <i class="fab fa-whatsapp"></i>
                </a>
                <a href="https://www.facebook.com/share/1cJEj3Qakg/" class="social-link facebook" target="_blank">
                    <i class="fab fa-facebook-f"></i>
                </a>
                <a href="https://www.instagram.com/bengkel_prastkakikaki?igsh=bmowamVweXA3cjU4" class="social-link instagram" target="_blank">
                    <i class="fab fa-instagram"></i>
                </a>
                <a href="https://www.tiktok.com/@prastkakikaki?_t=ZS-8xUTnDtwgdk&_r=1" class="social-link tiktok" target="_blank">
                    <i class="fab fa-tiktok"></i>
                </a>
            </div>
            
            <div class="copyright">
                <p>&copy; <span id="year"></span> Prast Kaki Kaki. All Rights Reserved.</p>
            </div>
        </div>
    </div>
</footer>

<style>
    /* ===== Footer Styles ===== */
    .footer {
        background: #0f172a;
        color: #e2e8f0;
        padding: 60px 0 0;
        font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        border-top: 1px solid #1e293b;
    }
    
    .container {
        max-width: 1200px;
        margin: 0 auto;
        padding: 0 20px;
    }
    
    /* Footer Grid Layout */
    .footer-grid {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
        gap: 40px;
        margin-bottom: 50px;
    }
    
    /* Profile Section */
    .footer-profile {
        display: flex;
        flex-direction: column;
    }
    
    .footer-title {
        font-size: 1.5rem;
        color: #3aa8ff;
        margin-bottom: 20px;
        position: relative;
        padding-bottom: 10px;
    }
    
    .footer-title::after {
        content: '';
        position: absolute;
        left: 0;
        bottom: 0;
        width: 50px;
        height: 2px;
        background: #3aa8ff;
    }
    
    .footer-description {
        line-height: 1.6;
        margin-bottom: 25px;
        color: #94a3b8;
    }
    
    .footer-contacts {
        display: flex;
        flex-direction: column;
        gap: 15px;
    }
    
    .contact-item {
        display: flex;
        gap: 15px;
        align-items: flex-start;
    }
    
    .contact-item i {
        color: #3aa8ff;
        font-size: 1.2rem;
        margin-top: 3px;
    }
    
    .contact-item h4 {
        color: #e2e8f0;
        margin-bottom: 5px;
        font-size: 1rem;
    }
    
    .contact-item p {
        color: #94a3b8;
        margin: 0;
        font-size: 0.9rem;
    }
    
    /* Links Section */
    .footer-links ul {
        list-style: none;
        padding: 0;
    }
    
    .footer-links li {
        margin-bottom: 12px;
    }
    
    .footer-links a {
        color: #94a3b8;
        text-decoration: none;
        transition: all 0.3s ease;
        display: inline-block;
        font-size: 0.95rem;
    }
    
    .footer-links a:hover {
        color: #3aa8ff;
        transform: translateX(5px);
    }
    
    /* Booking Form Styles */
    .footer-form {
        background: #1e293b;
        border-radius: 10px;
        padding: 25px;
        box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
    }
    
    .message-form {
        display: grid;
        gap: 15px;
    }
    
    .form-group {
        display: flex;
        flex-direction: column;
        gap: 8px;
    }
    
    .form-group label {
        color: #cbd5e1;
        font-size: 0.9rem;
        font-weight: 500;
    }
    
    .message-form input,
    .message-form select {
        padding: 12px 15px;
        border-radius: 8px;
        border: 1px solid #334155;
        background: #1e293b;
        color: #f8fafc;
        font-family: inherit;
        transition: all 0.3s ease;
        width: 100%;
    }
    
    .message-form input:focus,
    .message-form select:focus {
        outline: none;
        border-color: #3aa8ff;
        box-shadow: 0 0 0 2px rgba(58, 168, 255, 0.2);
    }
    
    /* Time Selection */
    .time-options {
        display: flex;
        gap: 10px;
    }
    
    .time-option {
        flex: 1;
        position: relative;
    }
    
    .time-option input {
        position: absolute;
        opacity: 0;
    }
    
    .time-option span {
        display: block;
        padding: 10px;
        border-radius: 6px;
        background: #1e293b;
        border: 1px solid #334155;
        text-align: center;
        cursor: pointer;
        transition: all 0.3s ease;
        font-size: 0.9rem;
    }
    
    .time-option input:checked + span {
        background: #3aa8ff;
        border-color: #3aa8ff;
        color: white;
    }
    
    /* Submit Button */
    .submit-btn {
        background: #25D366;
        color: white;
        border: none;
        padding: 14px;
        border-radius: 8px;
        cursor: pointer;
        font-weight: 600;
        transition: all 0.3s ease;
        display: flex;
        align-items: center;
        justify-content: center;
        gap: 10px;
        width: 100%;
        margin-top: 5px;
    }
    
    .submit-btn:hover {
        background: #128C7E;
        transform: translateY(-2px);
        box-shadow: 0 4px 12px rgba(37, 211, 102, 0.3);
    }
    
    /* Footer Bottom */
    .footer-bottom {
        border-top: 1px solid #1e293b;
        padding: 30px 0;
        display: flex;
        flex-direction: column;
        align-items: center;
        gap: 20px;
    }
    
    .social-links {
        display: flex;
        gap: 15px;
    }
    
    .social-link {
        width: 40px;
        height: 40px;
        border-radius: 50%;
        display: flex;
        align-items: center;
        justify-content: center;
        color: white;
        transition: all 0.3s ease;
    }
    
    .whatsapp { background: #25D366; }
    .facebook { background: #1877F2; }
    .instagram { 
        background: linear-gradient(45deg, #405DE6, #5851DB, #833AB4, #C13584, #E1306C, #FD1D1D); 
    }
    .tiktok { background: #000000; }
    
    .social-link:hover {
        transform: translateY(-3px) scale(1.1);
    }
    
    .copyright {
        color: #64748b;
        font-size: 0.9rem;
        text-align: center;
    }
    
    /* Responsive Adjustments */
    @media (max-width: 768px) {
        .footer-grid {
            grid-template-columns: 1fr;
            gap: 30px;
        }
        
        .time-options {
            flex-direction: column;
        }
        
        .footer-title {
            font-size: 1.3rem;
        }
    }
</style>

<script>
    // Auto-update copyright year
    document.getElementById('year').textContent = new Date().getFullYear();
    
    // Booking form handler
    document.getElementById('bookingForm').addEventListener('submit', function(e) {
        e.preventDefault();
        
        const formData = new FormData(this);
        const data = Object.fromEntries(formData);
        
        const message = `*BOOKING CEK GRATIS*%0A%0A` +
                        `*Nama*: ${data.nama}%0A` +
                        `*Cabang*: ${data.cabang}%0A` +
                        `*Waktu*: ${data.waktu}%0A` +
                        `*Mobil*: ${data.mobil}%0A` +
                        `*Plat*: ${data.plat}%0A%0A` +
                        `*Nomor WhatsApp*: ${data.whatsapp}%0A%0A` +
                        `_Mohon konfirmasi ketersediaan jadwalnya. Terima kasih._`;
        
        window.open(`https://wa.me/6281226298787?text=${message}`, '_blank');
    });
</script>
            </div>
        </div>
        
        <!-- CTA Section -->
        <div class="cta-section">
            <div class="cta-content">
                <h2>Butuh Bantuan Cepat?</h2>
                <p>Konsultasi gratis via WhatsApp dengan teknisi kami sekarang juga!</p>
                
                <a href="https://wa.me/6281226298787" class="cta-button" target="_blank">
                    <i class="fab fa-whatsapp"></i> Chat Sekarang
                    <span class="cta-badge">Respons 5 Menit</span>
                </a>
                
                <div class="social-links">
                    <a href="https://wa.me/6281226298787" class="social-link whatsapp" target="_blank">
                        <i class="fab fa-whatsapp"></i>
                    </a>
                    <a href="https://www.facebook.com/share/1cJEj3Qakg/" class="social-link facebook" target="_blank">
                        <i class="fab fa-facebook-f"></i>
                    </a>
                    <a href="https://www.instagram.com/bengkel_prastkakikaki?igsh=bmowamVweXA3cjU4" class="social-link instagram" target="_blank">
                        <i class="fab fa-instagram"></i>
                    </a>
                    <a href="https://www.tiktok.com/@prastkakikaki?_t=ZS-8xUTnDtwgdk&_r=1" class="social-link tiktok" target="_blank">
                        <i class="fab fa-tiktok"></i>
                    </a>
                </div>
            </div>
        </div>
        
        <!-- Copyright -->
        <div class="copyright">
            <p>&copy; 2025 Prast Kaki Kaki. All Rights Reserved.</p>
        </div>
    </div>
</footer>

<style>
    /* Footer Styles */
    .footer {
        background: #0a192f;
        color: #e6f1ff;
        padding: 60px 0 0;
        font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    }
    
    .footer-grid {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
        gap: 40px;
        margin-bottom: 50px;
    }
    
    .footer-title {
        font-size: 1.5rem;
        color: #64ffda;
        margin-bottom: 20px;
        position: relative;
        padding-bottom: 10px;
    }
    
    .footer-title::after {
        content: '';
        position: absolute;
        left: 0;
        bottom: 0;
        width: 50px;
        height: 2px;
        background: #64ffda;
    }
    
    .footer-description {
        line-height: 1.6;
        margin-bottom: 20px;
        color: #ccd6f6;
    }
    
    .contact-item {
        display: flex;
        gap: 15px;
        margin-bottom: 15px;
        align-items: flex-start;
    }
    
    .contact-item i {
        color: #64ffda;
        font-size: 1.2rem;
        margin-top: 3px;
    }
    
    .contact-item h4 {
        margin-bottom: 5px;
        color: #e6f1ff;
    }
    
    .contact-item p {
        color: #8892b0;
        margin: 0;
    }
    
    .footer-links ul {
        list-style: none;
        padding: 0;
    }
    
    .footer-links li {
        margin-bottom: 12px;
    }
    
    .footer-links a {
        color: #ccd6f6;
        text-decoration: none;
        transition: all 0.3s ease;
        display: inline-block;
    }
    
    .footer-links a:hover {
        color: #64ffda;
        transform: translateX(5px);
    }
    
    /* Contact Form */
    .message-form {
        display: grid;
        gap: 15px;
    }
    
    .message-form input,
    .message-form textarea {
        padding: 12px 15px;
        border-radius: 5px;
        border: 1px solid #233554;
        background: #112240;
        color: #e6f1ff;
        font-family: inherit;
        transition: all 0.3s ease;
    }
    
    .message-form input:focus,
    .message-form textarea:focus {
        outline: none;
        border-color: #64ffda;
        box-shadow: 0 0 0 2px rgba(100, 255, 218, 0.2);
    }
    
    .submit-btn {
        background: #0a192f;
        color: #64ffda;
        border: 1px solid #64ffda;
        padding: 12px 20px;
        border-radius: 5px;
        cursor: pointer;
        font-weight: 600;
        transition: all 0.3s ease;
        display: flex;
        align-items: center;
        justify-content: center;
        gap: 10px;
    }
    
    .submit-btn:hover {
        background: rgba(100, 255, 218, 0.1);
        transform: translateY(-3px);
    }
    
    /* CTA Section */
    .cta-section {
        background: linear-gradient(135deg, #112240 0%, #0a192f 100%);
        border-radius: 10px;
        padding: 40px;
        text-align: center;
        margin-bottom: 40px;
        border: 1px solid #233554;
        position: relative;
        overflow: hidden;
    }
    
    .cta-section::before {
        content: '';
        position: absolute;
        top: -50%;
        left: -50%;
        width: 200%;
        height: 200%;
        background: radial-gradient(circle, rgba(100, 255, 218, 0.1) 0%, transparent 70%);
        animation: rotate 15s linear infinite;
    }
    
    @keyframes rotate {
        100% {
            transform: rotate(360deg);
        }
    }
    
    .cta-content {
        position: relative;
        z-index: 1;
    }
    
    .cta-section h2 {
        font-size: 2rem;
        margin-bottom: 15px;
        color: #e6f1ff;
    }
    
    .cta-section p {
        color: #8892b0;
        margin-bottom: 25px;
        font-size: 1.1rem;
    }
    
    .cta-button {
        background: #64ffda;
        color: #0a192f;
        padding: 15px 30px;
        border-radius: 50px;
        text-decoration: none;
        font-weight: 600;
        display: inline-flex;
        align-items: center;
        gap: 10px;
        transition: all 0.3s ease;
        position: relative;
        overflow: hidden;
        margin-bottom: 25px;
        box-shadow: 0 5px 15px rgba(100, 255, 218, 0.3);
    }
    
    .cta-button:hover {
        transform: translateY(-5px);
        box-shadow: 0 8px 25px rgba(100, 255, 218, 0.4);
    }
    
    .cta-badge {
        position: absolute;
        top: -10px;
        right: -10px;
        background: #ff5555;
        color: white;
        padding: 3px 10px;
        border-radius: 20px;
        font-size: 0.7rem;
        font-weight: bold;
    }
    
    /* Social Links */
    .social-links {
        display: flex;
        justify-content: center;
        gap: 15px;
    }
    
    .social-link {
        width: 40px;
        height: 40px;
        border-radius: 50%;
        display: flex;
        align-items: center;
        justify-content: center;
        color: white;
        transition: all 0.3s ease;
    }
    
    .whatsapp { background: #25D366; }
    .facebook { background: #1877F2; }
    .instagram { background: linear-gradient(45deg, #405DE6, #5851DB, #833AB4, #C13584, #E1306C, #FD1D1D); }
    .tiktok { background: #000000; }
    
    .social-link:hover {
        transform: translateY(-5px) scale(1.1);
    }
    
    /* Copyright */
    .copyright {
        text-align: center;
        padding: 20px 0;
        border-top: 1px solid #233554;
        color: #8892b0;
        font-size: 0.9rem;
    }
    
    /* Responsive */
    @media (max-width: 768px) {
        .footer-grid {
            grid-template-columns: 1fr;
        }
        
        .cta-section {
            padding: 30px 20px;
        }
        
        .cta-section h2 {
            font-size: 1.5rem;
        }
    }
</style>
</body>
</html>
