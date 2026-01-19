<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>DR HS - Medical Consultation</title>
  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; }
    body {
      font-family: 'Segoe UI', Arial, sans-serif;
      background: #f0f8ff;
      color: #333;
      line-height: 1.6;
    }
    a { text-decoration: none; color: inherit; }

    /* Header */
    header {
      background: linear-gradient(90deg, #2b6cb0, #38b2ac);
      color: #fff;
      padding: 15px 30px;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }
    header h1 { font-size: 1.8rem; font-weight: bold; }
    nav ul {
      list-style: none;
      display: flex;
      gap: 20px;
    }
    nav ul li a {
      color: #fff;
      font-weight: bold;
      transition: color 0.3s;
    }
    nav ul li a:hover { color: #e0f2f1; }

    /* Hero */
    .hero {
      background: url('https://images.unsplash.com/photo-1588776814546-ec7c7c9a5a3e?auto=format&fit=crop&w=1350&q=80') no-repeat center/cover;
      height: 420px;
      display: flex;
      align-items: center;
      justify-content: center;
      color: #fff;
      text-align: center;
    }
    .hero h2 {
      font-size: 2.8rem;
      background: rgba(0,0,0,0.5);
      padding: 20px 30px;
      border-radius: 10px;
    }

    /* Sections */
    section {
      padding: 50px 20px;
      max-width: 1100px;
      margin: auto;
    }
    section h3 {
      text-align: center;
      margin-bottom: 30px;
      font-size: 2rem;
      color: #2b6cb0;
    }

    /* Services */
    .services {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 25px;
    }
    .service {
      background: #fff;
      padding: 20px;
      border-radius: 10px;
      box-shadow: 0 6px 12px rgba(0,0,0,0.1);
      text-align: center;
      transition: transform 0.3s;
    }
    .service:hover { transform: translateY(-5px); }
    .service img {
      width: 80px;
      margin-bottom: 15px;
    }
    .service h4 { margin-bottom: 10px; color: #38b2ac; }

    /* Consultation Form */
    form {
      background: #fff;
      padding: 30px;
      border-radius: 10px;
      box-shadow: 0 6px 12px rgba(0,0,0,0.1);
    }
    form label { display: block; margin-bottom: 6px; font-weight: bold; }
    form input, form textarea, form select {
      width: 100%;
      padding: 12px;
      margin-bottom: 18px;
      border: 1px solid #ccc;
      border-radius: 8px;
    }
    form button {
      background: #2b6cb0;
      color: #fff;
      border: none;
      padding: 14px 22px;
      border-radius: 8px;
      cursor: pointer;
      font-size: 1rem;
      transition: background 0.3s;
    }
    form button:hover { background: #22577a; }

    /* Footer */
    footer {
      background: linear-gradient(90deg, #2b6cb0, #38b2ac);
      color: #fff;
      text-align: center;
      padding: 18px;
      margin-top: 40px;
    }
  </style>
</head>
<body>

  <!-- Header -->
  <header>
    <h1>DR. HS</h1>
    <nav>
      <ul>
        <li><a href="#services">Services</a></li>
        <li><a href="#consultation">Consultation</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </header>

  <!-- Hero -->
  <section class="hero">
    <h2>Your Health, Our Priority</h2>
  </section>

  <!-- Services -->
  <section id="services">
    <h3>Our Services</h3>
    <div class="services">
      <div class="service">
        <img src="https://cdn-icons-png.flaticon.com/512/2966/2966486.png" alt="Consultation icon">
        <h4>General Consultation</h4>
        <p>Comprehensive health check-ups and personalized advice.</p>
      </div>
      <div class="service">
        <img src="https://cdn-icons-png.flaticon.com/512/2966/2966480.png" alt="Pediatrics icon">
        <h4>Pediatrics</h4>
        <p>Specialized care for infants, children, and adolescents.</p>
      </div>
      <div class="service">
        <img src="https://cdn-icons-png.flaticon.com/512/2966/2966502.png" alt="Dermatology icon">
        <h4>Dermatology</h4>
        <p>Skin care treatments and expert dermatological consultation.</p>
      </div>
      <div class="service">
        <img src="https://cdn-icons-png.flaticon.com/512/2966/2966492.png" alt="Cardiology icon">
        <h4>Cardiology</h4>
        <p>Heart health monitoring and preventive care.</p>
      </div>
    </div>
  </section>

  <!-- Consultation Form -->
  <section id="consultation">
    <h3>Book a Consultation</h3>
    <form>
      <label for="name">Full Name</label>
      <input type="text" id="name" name="name" required />

      <label for="email">Email</label>
      <input type="email" id="email" name="email" required />

      <label for="phone">Phone</label>
      <input type="tel" id="phone" name="phone" required />

      <label for="service">Select Service</label>
      <select id="service" name="service" required>
        <option value="">-- Choose a service --</option>
        <option>General Consultation</option>
        <option>Pediatrics</option>
        <option>Dermatology</option>
        <option>Cardiology</option>
      </select>

      <label for="message">Describe your concern</label>
      <textarea id="message" name="message" rows="4" required></textarea>

      <button type="submit">Submit Request</button>
    </form>
  </section>

  <!-- Contact -->
  <section id="contact">
    <h3>Contact Us</h3>
    <p style="text-align:center;">📍 Alpha 1,Greater Noida UP, India</p>
    <p style="text-align:center;">📞 +91 9894344672 | ✉️ drhs@clinic.com</p>
  </section>

  <!-- Footer -->
  <footer>
    <p>© 2025 DR HS Medical Consultation. All rights reserved.</p>
  </footer>
<script> window.chtlConfig = { chatbotId: "1113223913" } </script>
<script async data-id="1113223913" id="chtl-script" type="text/javascript" src="https://chatling.ai/js/embed.js"></script>
</body>
</html>
<source>
chatling
<source/>

