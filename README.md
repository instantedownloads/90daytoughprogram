<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>TOUGH by LifeMathMoney - Master Life, Wealth & Happiness</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&family=Playfair+Display:wght@700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <style>
        :root {
            --primary: #000000;
            --secondary: #FFD700;
            --accent: #C8102E;
            --light: #F8F8F8;
            --dark: #222222;
        }
        
        body {
            font-family: 'Montserrat', sans-serif;
            line-height: 1.6;
            color: var(--dark);
            margin: 0;
            padding: 0;
            background-color: white;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        header {
            background-color: var(--primary);
            color: white;
            padding: 20px 0;
            position: sticky;
            top: 0;
            z-index: 100;
        }
        
        .header-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .logo {
            font-family: 'Playfair Display', serif;
            font-size: 28px;
            font-weight: 700;
            color: var(--secondary);
        }
        
        nav ul {
            display: flex;
            list-style: none;
        }
        
        nav ul li {
            margin-left: 30px;
        }
        
        nav ul li a {
            color: white;
            text-decoration: none;
            font-weight: 600;
            transition: color 0.3s;
        }
        
        nav ul li a:hover {
            color: var(--secondary);
        }
        
        .hero {
            background: linear-gradient(rgba(0,0,0,0.7), rgba(0,0,0,0.7)), url('https://images.unsplash.com/photo-1543357480-c60d400e2ef9?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80');
            background-size: cover;
            background-position: center;
            color: white;
            padding: 100px 0;
            text-align: center;
        }
        
        .hero h1 {
            font-family: 'Playfair Display', serif;
            font-size: 48px;
            margin-bottom: 20px;
            color: var(--secondary);
        }
        
        .hero p {
            font-size: 20px;
            max-width: 700px;
            margin: 0 auto 30px;
        }
        
        .cta-button {
            display: inline-block;
            background: var(--secondary);
            color: var(--primary);
            padding: 15px 40px;
            text-decoration: none;
            font-weight: bold;
            border-radius: 30px;
            font-size: 18px;
            transition: all 0.3s;
            text-transform: uppercase;
            letter-spacing: 1px;
        }
        
        .cta-button:hover {
            background: white;
            transform: translateY(-3px);
            box-shadow: 0 10px 20px rgba(0,0,0,0.2);
        }
        
        .benefits {
            padding: 80px 0;
            background-color: var(--light);
        }
        
        .section-title {
            text-align: center;
            font-family: 'Playfair Display', serif;
            font-size: 36px;
            margin-bottom: 50px;
            color: var(--primary);
        }
        
        .benefits-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }
        
        .benefit-card {
            background: white;
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            text-align: center;
            transition: transform 0.3s;
        }
        
        .benefit-card:hover {
            transform: translateY(-10px);
        }
        
        .benefit-icon {
            font-size: 50px;
            color: var(--accent);
            margin-bottom: 20px;
        }
        
        .benefit-card h3 {
            font-size: 22px;
            margin-bottom: 15px;
            color: var(--primary);
        }
        
        .book-showcase {
            padding: 80px 0;
            display: flex;
            align-items: center;
        }
        
        .book-cover {
            width: 350px;
            box-shadow: 0 20px 40px rgba(0,0,0,0.3);
            border-radius: 5px;
            margin-right: 60px;
        }
        
        .book-content {
            flex: 1;
        }
        
        .book-content h2 {
            font-family: 'Playfair Display', serif;
            font-size: 36px;
            color: var(--primary);
            margin-bottom: 20px;
        }
        
        .book-content ul {
            margin: 30px 0;
            padding-left: 20px;
        }
        
        .book-content li {
            margin-bottom: 15px;
            position: relative;
            list-style-type: none;
            padding-left: 30px;
        }
        
        .book-content li:before {
            content: "✓";
            color: var(--accent);
            position: absolute;
            left: 0;
            font-weight: bold;
        }
        
        .testimonials {
            padding: 80px 0;
            background-color: var(--primary);
            color: white;
        }
        
        .testimonial-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }
        
        .testimonial-card {
            background: rgba(255,255,255,0.1);
            padding: 30px;
            border-radius: 10px;
        }
        
        .testimonial-text {
            font-style: italic;
            margin-bottom: 20px;
        }
        
        .testimonial-author {
            font-weight: bold;
        }
        
        .author-bio {
            padding: 80px 0;
            text-align: center;
        }
        
        .author-image {
            width: 150px;
            height: 150px;
            border-radius: 50%;
            object-fit: cover;
            margin-bottom: 20px;
            border: 5px solid var(--secondary);
        }
        
        .author-bio h2 {
            font-family: 'Playfair Display', serif;
            font-size: 36px;
            color: var(--primary);
            margin-bottom: 20px;
        }
        
        .author-bio p {
            max-width: 700px;
            margin: 0 auto 30px;
        }
        
        .social-links a {
            color: var(--primary);
            font-size: 24px;
            margin: 0 10px;
            transition: color 0.3s;
        }
        
        .social-links a:hover {
            color: var(--accent);
        }
        
        .pricing {
            padding: 80px 0;
            background-color: var(--light);
            text-align: center;
        }
        
        .price-box {
            background: white;
            padding: 40px;
            border-radius: 10px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
            display: inline-block;
            max-width: 500px;
        }
        
        .price {
            font-size: 48px;
            font-weight: bold;
            color: var(--accent);
            margin: 20px 0;
        }
        
        .guarantee {
            display: flex;
            align-items: center;
            justify-content: center;
            margin: 30px 0;
        }
        
        .guarantee-icon {
            font-size: 40px;
            color: var(--secondary);
            margin-right: 15px;
        }
        
        .faq {
            padding: 80px 0;
        }
        
        .faq-item {
            margin-bottom: 20px;
            border-bottom: 1px solid #eee;
            padding-bottom: 20px;
        }
        
        .faq-question {
            font-weight: bold;
            font-size: 20px;
            margin-bottom: 10px;
            color: var(--primary);
        }
        
        footer {
            background-color: var(--dark);
            color: white;
            padding: 50px 0 20px;
            text-align: center;
        }
        
        .footer-links {
            display: flex;
            justify-content: center;
            margin-bottom: 30px;
        }
        
        .footer-links a {
            color: white;
            margin: 0 15px;
            text-decoration: none;
        }
        
        .copyright {
            opacity: 0.7;
            font-size: 14px;
        }
        
        @media (max-width: 768px) {
            .header-content {
                flex-direction: column;
            }
            
            nav ul {
                margin-top: 20px;
            }
            
            nav ul li {
                margin: 0 10px;
            }
            
            .book-showcase {
                flex-direction: column;
            }
            
            .book-cover {
                margin-right: 0;
                margin-bottom: 40px;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="container header-content">
            <div class="logo">TOUGH</div>
            <nav>
                <ul>
                    <li><a href="#about">About</a></li>
                    <li><a href="#benefits">Benefits</a></li>
                    <li><a href="#testimonials">Success Stories</a></li>
                    <li><a href="#author">Author</a></li>
                    <li><a href="#pricing">Get It Now</a></li>
                </ul>
            </nav>
        </div>
    </header>
    
    <section class="hero">
        <div class="container">
            <h1>UNLOCK YOUR POTENTIAL</h1>
            <p>The ultimate guide to mental toughness, financial freedom, physical mastery, and unshakable happiness. Transform every aspect of your life with principles that work.</p>
            <a href="https://lifemathmoney.gumroad.com/l/tough" class="cta-button">Get Instant Access Now</a>
        </div>
    </section>
    
    <section id="benefits" class="benefits">
        <div class="container">
            <h2 class="section-title">What You'll Achieve</h2>
            <div class="benefits-grid">
                <div class="benefit-card">
                    <div class="benefit-icon">
                        <i class="fas fa-brain"></i>
                    </div>
                    <h3>Mental Mastery</h3>
                    <p>Develop unshakable focus, discipline, and resilience to overcome any obstacle life throws at you.</p>
                </div>
                <div class="benefit-card">
                    <div class="benefit-icon">
                        <i class="fas fa-chart-line"></i>
                    </div>
                    <h3>Financial Freedom</h3>
                    <p>Learn the money mindset and strategies that will 10x your income and build lasting wealth.</p>
                </div>
                <div class="benefit-card">
                    <div class="benefit-icon">
                        <i class="fas fa-dumbbell"></i>
                    </div>
                    <h3>Physical Power</h3>
                    <p>Build strength, stamina, and the physique you've always wanted with efficient training methods.</p>
                </div>
                <div class="benefit-card">
                    <div class="benefit-icon">
                        <i class="fas fa-heart"></i>
                    </div>
                    <h3>Emotional Control</h3>
                    <p>Master your emotions, eliminate anxiety, and cultivate deep, lasting happiness.</p>
                </div>
                <div class="benefit-card">
                    <div class="benefit-icon">
                        <i class="fas fa-users"></i>
                    </div>
                    <h3>Social Influence</h3>
                    <p>Develop charisma and leadership skills that make people naturally respect and follow you.</p>
                </div>
                <div class="benefit-card">
                    <div class="benefit-icon">
                        <i class="fas fa-clock"></i>
                    </div>
                    <h3>Time Mastery</h3>
                    <p>Learn productivity systems used by top performers to get 10x more done in half the time.</p>
                </div>
            </div>
        </div>
    </section>
    
    <section class="book-showcase">
        <div class="container">
            <img src="https://public-files.gumroad.com/variants/4t4h1q1q0j8z4q1z7o3p3x1d1b3w1/3293a5a5a5a5a5a5a5a5a5a5a5a5a5a5" alt="TOUGH Book Cover" class="book-cover">
            <div class="book-content">
                <h2>What's Inside TOUGH</h2>
                <p>The most comprehensive guide to self-mastery ever created, distilled into actionable principles you can implement immediately.</p>
                <ul>
                    <li>The 7 Pillars of Mental Toughness</li>
                    <li>Wealth Creation Blueprint</li>
                    <li>90-Day Body Transformation Protocol</li>
                    <li>Happiness Optimization Framework</li>
                    <li>Decision-Making Mastery</li>
                    <li>Stress Inoculation Training</li>
                    <li>Focus & Productivity Systems</li>
                    <li>Social Dominance Strategies</li>
                    <li>Life Purpose Discovery Process</li>
                    <li>And much more...</li>
                </ul>
                <a href="https://lifemathmoney.gumroad.com/l/tough" class="cta-button">Download Sample Chapter</a>
            </div>
        </div>
    </section>
    
    <section id="testimonials" class="testimonials">
        <div class="container">
            <h2 class="section-title" style="color: white;">Success Stories</h2>
            <div class="testimonial-grid">
                <div class="testimonial-card">
                    <div class="testimonial-text">
                        "After implementing the principles in TOUGH, I doubled my income in 6 months, lost 25lbs of fat, and finally have control over my emotions. This book is worth 100x the price."
                    </div>
                    <div class="testimonial-author">- Michael T., Entrepreneur</div>
                </div>
                <div class="testimonial-card">
                    <div class="testimonial-text">
                        "The mental toughness framework alone transformed how I approach challenges. I went from constantly stressed to handling high-pressure situations with ease. Life-changing."
                    </div>
                    <div class="testimonial-author">- Sarah K., Corporate Executive</div>
                </div>
                <div class="testimonial-card">
                    <div class="testimonial-text">
                        "I've read hundreds of self-help books, but TOUGH stands apart. The combination of practical strategies for wealth, health, and happiness is unmatched. My #1 recommendation."
                    </div>
                    <div class="testimonial-author">- David R., Fitness Coach</div>
                </div>
            </div>
        </div>
    </section>
    
    <section id="author" class="author-bio">
        <div class="container">
            <img src="https://images.unsplash.com/photo-1560250097-0b93528c311a?ixlib=rb-1.2.1&auto=format&fit=crop&w=300&q=80" alt="LifeMathMoney" class="author-image">
            <h2>About LifeMathMoney</h2>
            <p>For over a decade, LifeMathMoney has been helping men and women transform their lives through practical, no-BS strategies for success. A former engineer turned entrepreneur, investor, and peak performance coach, he's distilled decades of research and real-world experience into this comprehensive guide.</p>
            <p>His work has been featured in Forbes, Men's Health, and The Wall Street Journal, and has helped over 50,000 students achieve breakthrough results.</p>
            <div class="social-links">
                <a href="#"><i class="fab fa-twitter"></i></a>
                <a href="#"><i class="fab fa-instagram"></i></a>
                <a href="#"><i class="fab fa-youtube"></i></a>
            </div>
        </div>
    </section>
    
    <section id="pricing" class="pricing">
        <div class="container">
            <h2 class="section-title">Get TOUGH Today</h2>
            <div class="price-box">
                <h3>Complete TOUGH System</h3>
                <div class="price">$49</div>
                <p>Instant digital download (PDF, ePub, Mobi)</p>
                <p>Includes all future updates</p>
                <a href="https://lifemathmoney.gumroad.com/l/tough" class="cta-button">Buy Now</a>
                <div class="guarantee">
                    <div class="guarantee-icon">
                        <i class="fas fa-shield-alt"></i>
                    </div>
                    <div>30-Day 100% Money-Back Guarantee</div>
                </div>
            </div>
        </div>
    </section>
    
    <section class="faq">
        <div class="container">
            <h2 class="section-title">Frequently Asked Questions</h2>
            <div class="faq-item">
                <div class="faq-question">Is this book only for men?</div>
                <p>No! While the principles are presented in a straightforward, no-nonsense way that appeals particularly to men, the strategies work equally well for women. About 35% of our readers are women who appreciate the direct approach.</p>
            </div>
            <div class="faq-item">
                <div class="faq-question">How is this different from other self-help books?</div>
                <p>TOUGH cuts through the fluff and theory to deliver actionable systems you can implement immediately. Most books focus on one area (money OR fitness OR mindset) - this gives you the complete picture with integrated strategies that compound results.</p>
            </div>
            <div class="faq-item">
                <div class="faq-question">What format does the book come in?</div>
                <p>You'll get instant access to all three major ebook formats: PDF (for reading on computers/tablets), ePub (for Apple/iBooks, Nook, etc.), and Mobi (for Kindle).</p>
            </div>
            <div class="faq-item">
                <div class="faq-question">Is there a physical version available?</div>
                <p>Currently, TOUGH is only available in digital format. This allows us to keep the price affordable and update the content regularly. Many readers print the PDF at their local print shop if they prefer physical copies.</p>
            </div>
        </div>
    </section>
    
    <footer>
        <div class="container">
            <div class="logo" style="margin-bottom: 30px;">TOUGH</div>
            <div class="footer-links">
                <a href="#">Privacy Policy</a>
                <a href="#">Terms</a>
                <a href="#">Contact</a>
                <a href="#">Affiliates</a>
            </div>
            <div class="copyright">
                © 2023 LifeMathMoney. All rights reserved.
            </div>
        </div>
    </footer>
</body>
</html>
