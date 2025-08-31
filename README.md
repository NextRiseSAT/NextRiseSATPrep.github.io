<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>NEXT RISE SAT PREP - Boost Your Score Today</title>
<style>
  /* Reset and base */
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
    padding: 0;
  }
  /* Navigation */
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
    align-items: center;
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
  /* Page Sections */
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
    animation: fadeIn 0.6s ease-out;
  }
  /* Home Page */
  .hero {
    text-align: center;
    margin-bottom: 3rem;
  }
  .hero h1 {
    font-size: 3.5rem;
    color: #333;
    margin-bottom: 1rem;
    background: linear-gradient(135deg, #667eea, #764ba2);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
  }
  .hero p {
    font-size: 1.3rem;
    color: #666;
    margin-bottom: 2rem;
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
  .feature-icon {
    font-size: 3rem;
    margin-bottom: 1rem;
    color: #667eea;
  }
  /* About Page */
  .score-highlight {
    background: linear-gradient(135deg, #667eea, #764ba2);
    color: white;
    padding: 0.5rem 1rem;
    border-radius: 10px;
    display: inline-block;
    margin: 1rem 0;
    font-weight: bold;
  }
  ul {
    margin-top: 1rem;
    line-height: 1.8;
  }
  h3 {
    margin-top: 2rem;
    color: #667eea;
  }
  /* Services Page */
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
  .price {
    font-size: 2rem;
    color: #667eea;
    font-weight: bold;
    margin: 1rem 0;
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
  /* Testimonials Page */
  .testimonial {
    background: rgba(255, 255, 255, 0.8);
    padding: 2rem;
    border-radius: 15px;
    margin-bottom: 2rem;
    box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
  }
  .testimonial-text {
    font-style: italic;
    font-size: 1.1rem;
    margin-bottom: 1rem;
    color: #555;
  }
  .testimonial-author {
    font-weight: bold;
    color: #667eea;
  }
  .stars {
    color: #ffd700;
    font-size: 1.2rem;
    margin-bottom: 1rem;
  }
  /* Contact Page */
  .contact-content {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 2rem;
  }
  .contact-form {
    background: rgba(255,255,255,0.8);
    padding: 2rem;
    border-radius: 15px;
    box-shadow: 0 5px 15px rgba(0,0,0,0.1);
  }
  .contact-form h3 {
    color: #667eea;
    margin-bottom: 1.5rem;
  }
  form .form-group {
    margin-bottom: 1rem;
  }
  label {
    display: block;
    margin-bottom: 0.3rem;
  }
  input, textarea {
    width: 100%;
    padding: 0.6rem;
    border-radius: 6px;
    border: 1px solid #ccc;
    font-size: 1rem;
  }
  button.cta-button {
    margin-top: 1rem;
  }
  .contact-info {
    background: rgba(255,255,255,0.8);
    padding: 2rem;
    border-radius: 15px;
    box-shadow: 0 5px 15px rgba(0,0,0,0.1);
    display: flex;
    flex-direction: column;
    gap: 1rem;
  }
  .contact-item {
    display: flex;
    align-items: center;
    gap: 1rem;
  }
  .contact-icon {
    font-size: 1.8rem;
    color: #667eea;
  }
  .contact-item h4 {
    margin: 0;
    color: #667eea;
  }
  /* Quick start box */
  .quick-start {
    margin-top: 2rem;
    padding: 1.5rem;
    background: rgba(102, 126, 234, 0.1);
    border-radius: 10px;
  }
  .quick-start h4 {
    color: #667eea;
    margin-bottom: 1rem;
  }
  /* Mobile Responsiveness */
  @media (max-width: 768px) {
    .nav-links {
      flex-direction: column;
      gap: 0.5rem;
    }
    .hero h1 {
      font-size: 2.5rem;
    }
    .contact-content {
      grid-template-columns: 1fr;
    }
    .page-content {
      padding: 2rem;
    }
    iframe {
      width: 100% !important;
      height: auto !important;
    }
  }
  /* Animations */
  @keyframes fadeIn {
    from {
      opacity: 0;
      transform: translateY(30px);
    }
    to {
      opacity: 1;
      transform: translateY(0);
    }
  }
</style>
</head>
<body>
  <!-- Navigation -->
  <nav>
    <div class="container">
      <a href="#" class="logo" onclick="showPage('home', event)">NEXT RISE SAT PREP</a>
      <ul class="nav-links">
        <li><a href="#" onclick="showPage('home', event)" class="active">Home</a></li>
        <li><a href="#" onclick="showPage('about', event)">About</a></li>
        <li><a href="#" onclick="showPage('services', event)">Services & Pricing</a></li>
        <li><a href="#" onclick="showPage('testimonials', event)">Testimonials</a></li>
        <li><a href="#" onclick="showPage('contact', event)">Contact</a></li>
      </ul>
    </div>
  </nav>
  <!-- Home Page -->
  <div id="home" class="page active">
    <div class="container">
      <div class="page-content">
        <div class="hero">
          <h1>Boost Your SAT Score</h1>
          <p>Personalized tutoring that gets results. Join hundreds of students who've improved their scores.</p>
          <a href="#" class="cta-button" onclick="showPage('contact', event)">Get Started Today</a>
        </div>
        <div class="features">
          <div class="feature">
            <div class="feature-icon">📚</div>
            <h3>Personalized Learning</h3>
            <p>Every session is tailored to your unique strengths and weaknesses. We focus on what you need most.</p>
          </div>
          <div class="feature">
            <div class="feature-icon">📈</div>
            <h3>Proven Results</h3>
            <p>Our students see an average score increase of 100+ points with our targeted approach.</p>
          </div>
          <div class="feature">
            <div class="feature-icon">👥</div>
            <h3>Small Group Learning</h3>
            <p>Groups of 4-5 students create the perfect balance of personal attention and peer motivation.</p>
          </div>
        </div>
      </div>
    </div>
  </div>
  <!-- About Page -->
  <div id="about" class="page">
    <div class="container">
      <div class="page-content">
        <h2>About Your Tutor</h2>
        <div class="score-highlight">SAT Score: 1510/1600</div>
        <p>Hi I'm a passionate high schooler dedicated to helping students achieve their SAT goals. With my 1500+ SAT score and proven tutoring methods, I've helped over 150 students reach their target scores.</p>              
        <h3>My Qualifications:</h3>
        <ul>
          <li>SAT Score: 1510/1600 (Math: 780, Reading & Writing: 730)</li>
          <li>Extensive SAT tutoring experience</li>
          <li>Helped 50+ students improve their scores by an average of 250+ points</li>
          <li>Specialized in group learning dynamics and peer motivation</li>
        </ul>
        <h3>Why Choose Me?</h3>
        <p>I understand the SAT inside and out. I've not only excelled on the test myself but have spent years perfecting my teaching methods. I believe every student can succeed with the right approach, and I'm here to help you find yours.</p>
      </div>
    </div>
  </div>
  <!-- Services & Pricing Page -->
  <div id="services" class="page">
    <div class="container">
      <div class="page-content">
        <h2>Services & Pricing</h2>
        <p style="text-align: center; font-size: 1.1rem; color: #666; margin-bottom: 2rem;">Choose the package that works best for you. All sessions include personalized materials and practice tests.</p>    
        <div class="service-cards">
          <div class="service-card popular">
            <h3>Group SAT Prep Course</h3>
            <div class="price">$20/hour</div>
            <p style="color: #667eea; font-weight: bold;">8-Week Program</p>
            <ul style="text-align: left; margin: 1.5rem 0;">
              <li>Small groups of 4-5 students maximum</li>
              <li>16 total sessions (2 sessions per week)</li>
              <li>Each session: 1 hour 15 minutes</li>
              <li>Complete diagnostic assessment</li>
              <li>Custom study materials for each student</li>
              <li>Progress tracking and regular updates</li>
              <li>Peer learning and motivation</li>
            </ul>
            <div style="background: rgba(102, 126, 234, 0.1); padding: 1rem; border-radius: 10px; margin: 1rem 0;">
              <h4 style="color: #667eea; margin-bottom: 0.5rem;">Session Times:</h4>
              <p style="font-size: 0.9rem; margin: 0.25rem 0;"><strong>Tuesday & Thursday:</strong> 7:00 PM - 8:15 PM</p>
              <p style="font-size: 0.9rem; margin: 0.25rem 0;"><strong>Saturday & Sunday:</strong> 9:00 AM - 10:15 AM</p>
            </div>                        
            <div style="background: rgba(255, 255, 255, 0.8); padding: 1rem; border-radius: 10px; margin: 1rem 0;">
              <h4 style="color: #667eea; margin-bottom: 0.5rem;">Total Investment:</h4>
              <p style="font-size: 1.1rem; font-weight: bold;">$400 for complete 8-week program</p>
              <p style="font-size: 0.9rem; color: #666;">(16 sessions × 1.25 hours × $20/hour)</p>
            </div>                     
            <a href="#" class="cta-button" onclick="showPage('contact', event)">Join Next Group</a>
          </div>
        </div>
        </div>
      </div>
    </div>
  <!-- Testimonials Page -->
  <div id="testimonials" class="page">
    <div class="container">
      <div class="page-content">
        <h2>What Students Say</h2>
        <p style="text-align: center; font-size: 1.1rem; color: #666; margin-bottom: 2rem;">Don't just take our word for it. Here's what real students have to say about their experience.</p>   
        <div class="testimonial">
          <div class="stars">⭐⭐⭐⭐⭐</div>
          <p class="testimonial-text">"I went from 1200 to 1480 in just 8 weeks! The personalized approach really made the difference. Every session was focused on exactly what I needed to improve."</p>
          <p class="testimonial-author">— Sarah M., Senior at Westfield High</p>
        </div>
        <div class="testimonial">
          <div class="stars">⭐⭐⭐⭐⭐</div>
          <p class="testimonial-text">"The math section was my biggest weakness, but after working together, I scored an 800! The strategies and practice problems were exactly what I needed."</p>
          <p class="testimonial-author">— David L., Junior at Lincoln Academy</p>
        </div>
        <div class="testimonial">
          <div class="stars">⭐⭐⭐⭐⭐</div>
          <p class="testimonial-text">"Not only did my score improve by 300 points, but I actually felt confident going into the test. The practice tests and feedback were incredibly helpful."</p>
          <p class="testimonial-author">— Emma R., Senior at Roosevelt High</p>
        </div>
      </div>
    </div>
  </div>
  <!-- Contact Page -->
  <div id="contact" class="page">
    <div class="container">
      <div class="page-content">
        <h2>Contact Us</h2>
        <p>Ready to start improving your SAT score? Fill out the form below and we'll get back to you within 24 hours.</p>
        <iframe src="https://docs.google.com/forms/d/e/1FAIpQLScDTchvSs_W9eXijtJ2yBK9_s7_ZNVMhN9xJf_n-ohE5dR_Rg/viewform?embedded=true" width="640" height="1040" frameborder="0" marginheight="0" marginwidth="0">Loading…</iframe>
        <!-- Removed invalid </form> tag here -->
        <div class="contact-info">
          <div class="contact-item">
            <div class="contact-icon">📧</div>
            <div>
              <h4>Email</h4>
              <p>nextrisesatprep@gmail.com</p>
            </div>
          </div>
          <div class="contact-item">
            <div class="contact-icon">📍</div>
            <div>
              <h4>Location</h4>
              <p>Online (Anywhere)</p>
            </div>
          </div>
          <div class="contact-item">
            <div class="contact-icon">📅</div>
            <div>
              <h4>Availability</h4>
              <p>Tuesday to Sunday, 7 AM - 9 PM EST</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
<script>
  // Show the selected page and update nav active state
  function showPage(pageId, event) {
    event.preventDefault();
    const pages = document.querySelectorAll('.page');
    pages.forEach(page => {
      if (page.id === pageId) {
        page.classList.add('active');
      } else {
        page.classList.remove('active');
      }
    });
    // Update nav link active state
    const navLinks = document.querySelectorAll('.nav-links a');
    navLinks.forEach(link => {
      if (link.getAttribute('onclick').includes(pageId)) {
        link.classList.add('active');
      } else {
        link.classList.remove('active');
      }
    });
  }
</script>
</body>
</html>
