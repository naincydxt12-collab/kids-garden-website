# kids-garden-website
your kids will thank you ,when they will grow up.
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Kids Garden Play School - Nurturing Young Minds</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Arial', sans-serif;
            line-height: 1.6;
            color: #333;
            overflow-x: hidden;
        }

        /* Header */
        header {
            background: linear-gradient(135deg, #ff9a9e 0%, #fecfef 50%, #fecfef 100%);
            padding: 1rem 0;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }

        nav {
            max-width: 1200px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 0 2rem;
        }

        .logo {
            font-size: 2rem;
            font-weight: bold;
            color: #d63384;
            text-decoration: none;
        }

        .nav-links {
            display: flex;
            list-style: none;
            gap: 2rem;
        }

        .nav-links a {
            text-decoration: none;
            color: #333;
            font-weight: 500;
            transition: color 0.3s;
        }

        .nav-links a:hover {
            color: #d63384;
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(rgba(255,154,158,0.9), rgba(254,207,239,0.9)), 
                        url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1200 600"><rect fill="%23f8f9fa" width="1200" height="600"/><circle fill="%23ff9a9e" opacity="0.3" cx="200" cy="150" r="80"/><circle fill="%23fecfef" opacity="0.4" cx="800" cy="200" r="100"/><circle fill="%23d63384" opacity="0.2" cx="1000" cy="400" r="60"/><path fill="%23ff6b6b" opacity="0.3" d="M300 450 Q400 500 500 450 Q600 400 700 450"/></svg>');
            height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            color: white;
            margin-top: 80px;
        }

        .hero-content h1 {
            font-size: 4rem;
            margin-bottom: 1rem;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
        }

        .hero-content p {
            font-size: 1.5rem;
            margin-bottom: 2rem;
        }

        .cta-button {
            display: inline-block;
            background: #d63384;
            color: white;
            padding: 1rem 2rem;
            text-decoration: none;
            border-radius: 50px;
            font-size: 1.2rem;
            font-weight: bold;
            transition: all 0.3s;
            box-shadow: 0 4px 15px rgba(214,51,132,0.4);
        }

        .cta-button:hover {
            transform: translateY(-3px);
            box-shadow: 0 6px 20px rgba(214,51,132,0.6);
        }

        /* Sections */
        .section {
            padding: 5rem 2rem;
            max-width: 1200px;
            margin: 0 auto;
        }

        .section h2 {
            font-size: 3rem;
            text-align: center;
            margin-bottom: 3rem;
            color: #d63384;
        }

        /* About Section */
        .about {
            background: #f8f9fa;
        }

        .about-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 4rem;
            align-items: center;
        }

        .about-text p {
            font-size: 1.2rem;
            margin-bottom: 1.5rem;
            text-align: justify;
        }

        .about-image {
            text-align: center;
        }

        .about-image img {
            max-width: 100%;
            border-radius: 20px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.2);
        }

        /* Features */
        .features {
            background: white;
        }

        .features-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }

        .feature-card {
            text-align: center;
            padding: 2rem;
            border-radius: 20px;
            box-shadow: 0 5px 20px rgba(0,0,0,0.1);
            transition: transform 0.3s;
        }

        .feature-card:hover {
            transform: translateY(-10px);
        }

        .feature-icon {
            font-size: 4rem;
            margin-bottom: 1rem;
        }

        /* Programs */
        .programs {
            background: linear-gradient(135deg, #ff9a9e 0%, #fecfef 100%);
            color: white;
        }

        .programs-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
        }

        .program-card {
            background: rgba(255,255,255,0.2);
            padding: 2rem;
            border-radius: 20px;
            backdrop-filter: blur(10px);
            text-align: center;
        }

        /* Contact */
        .contact {
            background: #f8f9fa;
        }

        .contact-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 4rem;
        }

        .contact-info h3 {
            color: #d63384;
            margin-bottom: 1rem;
        }

        .contact-form {
            background: white;
            padding: 2rem;
            border-radius: 20px;
            box-shadow: 0 5px 20px rgba(0,0,0,0.1);
        }

        .form-group {
            margin-bottom: 1.5rem;
        }

        .form-group input,
        .form-group textarea {
            width: 100%;
            padding: 1rem;
            border: 2px solid #eee;
            border-radius: 10px;
            font-size: 1rem;
        }

        .form-group input:focus,
        .form-group textarea:focus {
            outline: none;
            border-color: #d63384;
        }

        /* Footer */
        footer {
            background: #333;
            color: white;
            text-align: center;
            padding: 2rem;
        }

        /* Responsive */
        @media (max-width: 768px) {
            .nav-links {
                display: none;
            }

            .hero-content h1 {
                font-size: 2.5rem;
            }

            .about-content,
            .contact-content {
                grid-template-columns: 1fr;
            }

            .section {
                padding: 3rem 1rem;
            }
        }

        /* Animations */
        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .animate {
            animation: fadeInUp 0.8s ease forwards;
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <nav>
            <a href="#" class="logo">🌸 Kids Garden</a>
            <ul class="nav-links">
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#programs">Programs</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <!-- Hero Section -->
    <section id="home" class="hero">
        <div class="hero-content animate">
            <h1>Welcome to Kids Garden</h1>
            <p>Where Little Hearts Blossom into Bright Minds</p>
            <a href="#contact" class="cta-button">Enroll Now</a>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="section about">
        <h2 class="animate">About Our Play School</h2>
        <div class="about-content">
            <div class="about-text animate">
                <p>At Kids Garden Play School, we create a nurturing environment where children aged 2-5 years can explore, learn, and grow through play. Our experienced teachers use child-centered approaches to foster creativity, social skills, and cognitive development.</p>
                <p>With small class sizes and a low teacher-to-child ratio, every child receives individual attention and care. Our curriculum is designed to spark curiosity and build confidence through hands-on learning experiences.</p>
            </div>
            <div class="about-image animate">
                <img src="data:image/svg+xml,<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 400 300'><rect fill='%23ff9a9e' rx='20' x='50' y='50' width='300' height='200'/><circle fill='%23fecfef' cx='150' cy='120' r='40'/><circle fill='%23d63384' cx='250' cy='100' r='30'/><rect fill='%23ff6b6b' x='100' y='180' width='60' height='80' rx='10'/><rect fill='%23ff9a56' x='220' y='170' width='50' height='90' rx='8'/><path fill='%234ecdc4' d='M80 250 Q120 230 160 260 Q200 240 240 270 Q280 250 320 280'/></svg>" alt="Happy children playing">
            </div>
        </div>
    </section>

    <!-- Features Section -->
    <section class="section features">
        <h2 class="animate">Why Choose Us?</h2>
        <div class="features-grid">
            <div class="feature-card animate">
                <div class="feature-icon">🎨</div>
                <h3>Creative Learning</h3>
                <p>Art, music, and storytelling to spark imagination and self-expression.</p>
            </div>
            <div class="feature-card animate">
                <div class="feature-icon">🌱</div>
                <h3>Nature Play</h3>
                <p>Outdoor adventures and gardening to connect with nature.</p>
            </div>
            <div class="feature-card animate">
                <div class="feature-icon">👫</div>
                <h3>Small Classes</h3>
                <p>Personal attention with low teacher-to-child ratios.</p>
            </div>
            <div class="feature-card animate">
                <div class="feature-icon">🏆</div>
                <h3>Safe Environment</h3>
                <p>Secure campus with CCTV and trained staff.</p>
            </div>
        </div>
    </section>

    <!-- Programs Section -->
    <section id="programs" class="section programs">
        <h2 class="animate">Our Programs</h2>
        <div class="programs-grid">
            <div class="program-card animate">
                <h3>Playgroup (2-3 yrs)</h3>
                <p>Introduction to social skills, basic motor development, and sensory play.</p>
            </div>
            <div class="program-card animate">
                <h3>Nursery (3-4 yrs)</h3>
                <p>Pre-literacy, numeracy, and creative expression through structured play.</p>
            </div>
            <div class="program-card animate">
                <h3>LKG (4-5 yrs)</h3>
                <p>School readiness program with phonics, numbers, and life skills.</p>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="section contact">
        <h2 class="animate">Get In Touch</h2>
        <div class="contact-content">
            <div class="contact-info animate">
                <h3>📍 Visit Us</h3>
                <p><strong>Address:</strong><br>Green Valley, Blossom Road<br>City Center, 123456</p>
                <p><strong>Phone:</strong><br>+1 (555) 123-4567</p>
                <p><strong>Email:</strong><br>info@kidsgardenplayschool.com</p>
                <p><strong>Hours:</strong><br>Mon-Fri: 8AM - 5PM</p>
            </div>
            <div class="contact-form animate">
                <form>
                    <div class="form-group">
                        <input type="text" placeholder="Your Name" required>
                    </div>
                    <div class="form-group">
                        <input type="email" placeholder="Your Email" required>
                    </div>
                    <div class="form-group">
                        <input type="tel" placeholder="Your Phone">
                    </div>
                    <div class="form-group">
                        <textarea rows="5" placeholder="Your Message"></textarea>
                    </div>
                    <button type="submit" class="cta-button" style="width: 100%; margin-top: 1rem;">Send Message</button>
                </form>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <p>&copy; 2024 Kids Garden Play School. All rights reserved. | Nurturing Tomorrow's Leaders Today 🌸</p>
    </footer>

    <script>
        // Smooth scrolling for navigation links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({
                        behavior: 'smooth',
                        block: 'start'
                    });
                }
            });
        });

        // Form submission
        document.querySelector('form').addEventListener('submit', function(e) {
            e.preventDefault();
            alert('Thank you for your message! We will get back to you soon. 🌸');
            this.reset();
        });

        // Add animation on scroll
        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.style.animationDelay = '0.2s';
                    entry.target.classList.add('animate');
                }
            });
        });

        document.querySelectorAll('.animate').forEach(el => {
            observer.observe(el);
        });
    </script>
</body>
</html>
