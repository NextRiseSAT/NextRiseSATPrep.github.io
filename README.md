<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Elite SAT Tutoring - Boost Your Score Today</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: #333;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        nav {
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            position: fixed;
            top: 0;
            width: 100%;
            z-index: 1000;
            box-shadow: 0 2px 20px rgba(0, 0, 0, 0.1);
        }

        nav .container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1rem 20px;
        }

        .logo {
            font-size: 1.8rem;
            font-weight: bold;
            color: #667eea;
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
            transition: color 0.3s ease;
            cursor: pointer;
            padding: 0.5rem 1rem;
            border-radius: 5px;
        }

        .nav-links a:hover,
        .nav-links a.active {
            color: #667eea;
            background: rgba(102, 126, 234, 0.1);
        }

        .page {
            display: none;
            padding: 120px 0 80px;
            min-height: 100vh;
        }

        .page.active {
            display: block;
        }

        .page-content {
            background: rgba(255, 255, 255, 0.95);
            border-radius: 20px;
            padding: 3rem;
            margin-bottom: 2rem;
            box-shadow: 0 15px 35px rgba(0, 0, 0, 0.1);
            backdrop-filter: blur(10px);
        }

        .hero {
            text-align: center;
            margin-bottom: 3rem;
        }

        .hero h1 {
            font-size: 3.5rem;
            background: linear-gradient(135deg, #667eea, #764ba2);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        .cta-button {
            display: inline-block;
            background: linear-gradient(135deg, #667eea, #764ba2);
            color: white;
            padding: 1rem 2rem;
            text-decoration: none;
            border-radius: 50px;
            font-weight: bold;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            box-shadow: 0 5px 15px rgba(102, 126, 234, 0.4);
        }

        .cta-button:hover {
            transform: translateY(-2px);
            box-shadow: 0 8px 25px rgba(102, 126, 234, 0.6);
        }

        .features {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin-top: 3rem;
        }

        .feature {
            text-align: center;
            padding: 2rem;
            background: rgba(255, 255, 255, 0.5);
            border-radius: 15px;
            transition: transform 0.3s ease;
        }

        .feature:hover {
            transform: translateY(-5px);
        }

        .service-cards {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 2rem;
            margin-top: 2rem;
        }

        .service-card {
            background: rgba(255, 255, 255, 0.8);
            border-radius: 15px;
            padding: 2rem;
            text-align: center;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .service-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.15);
        }

        .popular {
            position: relative;
            border: 3px solid #667eea;
        }

        .popular::before {
            content: "Most Popular";
            position: absolute;
            top: -15px;
            left: 50%;
            transform: translateX(-50%);
            background: #667eea;
            color: white;
            padding: 0.5rem 1rem;
            border-radius: 20px;
            font-size: 0.9rem;
        }

        .testimonial {
            background: rgba(255, 255, 255, 0.8);
            padding: 2rem;
            border-radius: 15px;
            margin-bottom: 2rem;
        }

        .contact-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 3rem;
        }

        @media (max-width: 768px) {
            .contact-content {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <!-- Navigation -->
    <nav>
        <div class="container">
            <a href="#" class="logo">Elite SAT Tutoring</a>
            <ul class="nav-links">
                <li><a href="#" onclick="showPage('home')">Home</a></li>
                <li><a href="#" onclick="showPage('about')">About</a></li>
                <li><a href="#" onclick="showPage('services')">Services & Pricing</a></li>
                <li><a href="#" onclick="showPage('testimonials')">Testimonials</a></li>
                <li><a href="#" onclick="showPage('contact')">Contact</a></li>
            </ul>
        </div>
    </nav>

    <!-- Home -->
    <div id="home" class="page active">
        <div class="container">
            <div class="page-content">
                <div class="hero">
                    <h1>Boost Your SAT Score</h1>
                    <p>Personalized tutoring that gets results. Join hundreds of students who've improved their scores by 200+ points.</p>
                    <a href="#" class="cta-button" onclick="showPage('contact')">Get Started Today</a>
                </div>
                <div class="features">
                    <div class="feature">📚 Personalized Learning</div>
                    <div class="feature">📈 Proven Results</div>
                    <div class="feature">👥 Small Group Learning</div>
                </div>
            </div>
        </div>
    </div>

    <!-- About -->
    <div id="about" class="page">
        <div class="container">
            <div class="page-content">
                <h2>About Your Tutor</h2>
                <p>Hi! I'm [Your Name], SAT score 1510/1600, and I've helped over 150 students improve their scores by an average of 250+ points.</p>
            </div>
        </div>
    </div>

    <!-- Services -->
    <div id="services" class="page">
        <div class="container">
            <div class="page-content">
                <h2>Services & Pricing</h2>
                <div class="service-cards">
                    <div class="service-card popular">
                        <h3>Group SAT Prep</h3>
                        <p>$20/hour - 8 Week Program</p>
                        <a href="#" class="cta-button" onclick="showPage('contact')">Join Now</a>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <!-- Testimonials -->
    <div id="testimonials" class="page">
        <div class="container">
            <div class="page-content">
                <h2>What Students Say</h2>
                <div class="testimonial">⭐⭐⭐⭐⭐ "I went from 1200 to 1480 in 8 weeks!"</div>
            </div>
        </div>
    </div>

    <!-- Contact -->
    <div id="contact" class="page">
        <div class="container">
            <div class="page-content">
                <h2>Contact</h2>
                <div class="contact-content">
                    <div>
                        <form>
                            <label>Name</label><input type="text" required>
                            <label>Email</label><input type="email" required>
                            <button type="submit" class="cta-button">Send</button>
                        </form>
                    </div>
                    <div>
                        <p>📧 nextrisesatprep@mail.com</p>
                        <p>📱 (469) 740-6196</p>
                        <p>🌐 Online Sessions</p>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <script>
        function showPage(pageId) {
            document.querySelectorAll('.page').forEach(p => p.classList.remove('active'));
            document.getElementById(pageId).classList.add('active');

            document.querySelectorAll('.nav-links a').forEach(link => link.classList.remove('active'));
            document.querySelectorAll('.nav-links a').forEach(link => {
                if (link.getAttribute('onclick') === `showPage('${pageId}')`) {
                    link.classList.add('active');
                }
            });

            window.scrollTo(0, 0);
        }

        document.addEventListener('DOMContentLoaded', () => {
            document.querySelector('.nav-links a').classList.add('active');
        });

        document.querySelector('form').addEventListener('submit', function(e) {
            e.preventDefault();
            alert("Thanks! I'll respond within 24 hours.");
            this.reset();
        });
    </script>
</body>
</html>
