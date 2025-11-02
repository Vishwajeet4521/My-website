<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>THE HIMALAYAN INFRASTRUCTURE VALLEY</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700&display=swap" rel="stylesheet">
  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; }
    body { font-family: 'Poppins', sans-serif; background: #f7f9fc; color: #333; }

    /* Navbar */
    header {
      background: linear-gradient(90deg, #ff6a00, #ee0979);
      color: white;
      padding: 20px;
      text-align: center;
      position: sticky;
      top: 0;
      z-index: 1000;
      box-shadow: 0 4px 12px rgba(0,0,0,0.3);
    }
    header h1 { font-size: 2em; animation: glow 2s infinite alternate; }
    @keyframes glow {
      from { text-shadow: 0 0 10px #fff, 0 0 20px #ff6a00; }
      to { text-shadow: 0 0 20px #fff, 0 0 30px #ee0979; }
    }
    nav { margin-top: 10px; }
    nav a {
      color: white; margin: 0 10px; text-decoration: none;
      font-weight: 600; padding: 8px 14px; border-radius: 8px;
      transition: 0.3s; background: rgba(255,255,255,0.15);
    }
    nav a:hover { background: white; color: #ee0979; }

    /* Hero Slideshow */
    #home {
      height: 90vh; display: flex; justify-content: center; align-items: center;
      color: white; text-align: center; position: relative; overflow: hidden;
    }
    .slide {
      position: absolute; top: 0; left: 0; width: 100%; height: 100%;
      display: flex; flex-direction: column; justify-content: center; align-items: center;
      background-size: cover; background-position: center;
      transition: opacity 1s ease-in-out;
      opacity: 0;
    }
    .slide.active { opacity: 1; }
    .slide h1 { font-size: 3em; margin-bottom: 15px; text-shadow: 2px 2px 6px rgba(0,0,0,0.6); }
    .slide p { font-size: 1.3em; font-weight: 500; }

    /* Sections */
    section {
      max-width: 1100px; margin: 50px auto; padding: 30px 20px;
      background: white; border-radius: 20px;
      box-shadow: 0 6px 18px rgba(0,0,0,0.2);
    }
    h2 { text-align: center; color: #ee0979; margin-bottom: 20px; font-size: 2em; }

    /* Services */
    .services-grid {
      display: grid; grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
      gap: 20px;
    }
    .service-card {
      background: linear-gradient(135deg,#ffecd2,#fcb69f);
      padding: 25px; border-radius: 16px;
      text-align: center; font-weight: 500;
      transition: transform 0.4s, box-shadow 0.4s;
    }
    .service-card:nth-child(2) { background: linear-gradient(135deg,#a1c4fd,#c2e9fb); }
    .service-card:nth-child(3) { background: linear-gradient(135deg,#fccb90,#d57eeb); }
    .service-card:nth-child(4) { background: linear-gradient(135deg,#fbc2eb,#a6c1ee); }
    .service-card:hover { transform: translateY(-10px); box-shadow: 0 8px 20px rgba(0,0,0,0.3); }
    .service-card h3 { margin-bottom: 10px; color: #333; }

    /* Forms */
    form input, form select, form button {
      width: 100%; padding: 14px; margin: 10px 0;
      border-radius: 10px; border: none; font-size: 1em;
      box-shadow: 0 2px 6px rgba(0,0,0,0.2);
    }
    form button {
      background: linear-gradient(90deg,#ff6a00,#ee0979);
      color: white; cursor: pointer; font-weight: 700;
      transition: transform 0.3s;
    }
    form button:hover { transform: scale(1.05); }

    /* Payment */
    .upi-button {
      display: inline-block; padding: 14px 30px;
      background: linear-gradient(90deg,#43e97b,#38f9d7);
      color: #1b263b; font-weight: bold; border-radius: 12px;
      text-decoration: none; box-shadow: 0 4px 10px rgba(0,0,0,0.2);
      transition: transform 0.3s;
    }
    .upi-button:hover { transform: scale(1.1); }

    footer {
      background: linear-gradient(90deg,#ee0979,#ff6a00);
      color: white; text-align: center;
      padding: 20px; margin-top: 40px;
      border-radius: 20px 20px 0 0;
    }

    @media(max-width:768px){
      .slide h1 { font-size: 2em; }
      .slide p { font-size: 1em; }
    }
  </style>
</head>
<body>

  <header>
    <h1>THE HIMALAYAN INFRASTRUCTURE VALLEY</h1>
    <nav>
      <a href="#home">Home</a>
      <a href="#about">About</a>
      <a href="#services">Services</a>
      <a href="#contact">Contact</a>
      <a href="#login">Login/Signup</a>
      <a href="#payment">Payment</a>
    </nav>
  </header>

  <!-- Hero Slideshow -->
  <section id="home">
    <div class="slide active" style="background-image:url('https://picsum.photos/id/1018/1600/900');">
      <h1>Connecting You to the Future</h1>
      <p>Fast, Secure & Reliable Internet Solutions</p>
    </div>
    <div class="slide" style="background-image:url('https://picsum.photos/id/1015/1600/900');">
      <h1>Building Digital Infrastructure</h1>
      <p>Trusted Partner with 6+ Years of Expertise</p>
    </div>
  </section>

  <!-- About -->
  <section id="about">
    <h2>About Us</h2>
    <p style="text-align:center; font-size:1.1em;">
      We provide world-class Internet, networking, and OFC solutions. With over 6 years of expertise 
      alongside BSNL, we aim to bring seamless connectivity and modern infrastructure 
      for homes and businesses.
    </p>
  </section>

  <!-- Services -->
  <section id="services">
    <h2>Our Services</h2>
    <div class="services-grid">
      <div class="service-card">
        <h3>🌐 WIFI Internet</h3>
        <p>Lightning-fast and reliable WiFi connections.</p>
      </div>
      <div class="service-card">
        <h3>🔗 Leased Circuit</h3>
        <p>Dedicated high-speed lines for businesses.</p>
      </div>
      <div class="service-card">
        <h3>📹 CCTV Installation</h3>
        <p>Secure your property with smart surveillance.</p>
      </div>
      <div class="service-card">
        <h3>⚡ FTTH Broadband</h3>
        <p>Fiber-to-the-home for unmatched speed.</p>
      </div>
    </div>
  </section>

  <!-- Contact -->
  <section id="contact">
    <h2>Contact Us</h2>
    <p style="text-align:center;">
      📧 Email: <strong>thehivalley@gmail.com</strong> | 📱 WhatsApp: 
      <a href="https://wa.me/919934716124" target="_blank"><strong>+91 9934716124</strong></a>
    </p>
    <form action="https://formsubmit.co/thehivalley@gmail.com" method="POST">
      <input type="hidden" name="_captcha" value="false">
      <input type="hidden" name="_template" value="table">
      <input type="text" name="name" placeholder="Full Name" required>
      <select name="service" required>
        <option value="">Select Service</option>
        <option value="wifi">WIFI INTERNET</option>
        <option value="leased">LEASED CIRCUIT</option>
        <option value="cctv">CCTV CAMERA</option>
        <option value="ftth">FTTH</option>
      </select>
      <input type="email" name="email" placeholder="Email" required>
      <input type="tel" name="phone" placeholder="Phone Number" required>
      <input type="tel" name="whatsapp" placeholder="WhatsApp Number" required>
      <button type="submit">Send Request</button>
    </form>
  </section>

  <!-- Login -->
  <section id="login">
    <h2>Login / Signup</h2>
    <div style="display:flex; flex-wrap:wrap; gap:20px; justify-content:center;">
      <!-- Login -->
      <form id="loginForm" style="flex:1; min-width:280px; max-width:350px;">
        <h3>Login</h3>
        <input type="email" id="loginEmail" placeholder="Email" required>
        <input type="password" id="loginPassword" placeholder="Password" required>
        <button type="submit">Login</button>
      </form>

      <!-- Signup -->
      <form id="signupForm" style="flex:1; min-width:280px; max-width:350px;">
        <h3>Signup</h3>
        <input type="email" id="signupEmail" placeholder="Email" required>
        <input type="password" id="signupPassword" placeholder="Password" required>
        <button type="submit">Sign Up</button>
      </form>
    </div>
  </section>

  <!-- Payment -->
  <section id="payment">
    <h2>Make a Secure Payment</h2>
    <p style="text-align:center;">Click below to pay via UPI</p>
    <div style="text-align:center;">
      <a class="upi-button" href="upi://pay?pa=rns1252@okhdfcbank&pn=THE HIMALAYAN INFRASTRUCTURE VALLEY&cu=INR" target="_blank">
        💳 Pay Now via UPI
      </a>
    </div>
    <p style="text-align:center; margin-top:15px;">UPI ID: <strong>rns1252@okhdfcbank</strong></p>
    <p style="text-align:center; color:red; font-weight:bold;">
      ⚠️ Verify UPI ID before payment.
    </p>
  </section>

  <footer>
    <p>&copy; 2025 THE HIMALAYAN INFRASTRUCTURE VALLEY. All rights reserved.</p>
  </footer>

  <!-- Slideshow Script -->
  <script>
    let slides = document.querySelectorAll('.slide');
    let index = 0;
    setInterval(() => {
      slides[index].classList.remove('active');
      index = (index + 1) % slides.length;
      slides[index].classList.add('active');
    }, 4000);
  </script>

  <!-- Firebase Authentication Script -->
  <script type="module">
    import { initializeApp } from "https://www.gstatic.com/firebasejs/11.0.1/firebase-app.js";
    import { getAuth, createUserWithEmailAndPassword, signInWithEmailAndPassword } 
      from "https://www.gstatic.com/firebasejs/11.0.1/firebase-auth.js";

    const firebaseConfig = {
      apiKey: "YOUR_API_KEY",
      authDomain: "YOUR_PROJECT_ID.firebaseapp.com",
      projectId: "YOUR_PROJECT_ID",
      storageBucket: "YOUR_PROJECT_ID.appspot.com",
      messagingSenderId: "YOUR_SENDER_ID",
      appId: "YOUR_APP_ID"
    };

    const app = initializeApp(firebaseConfig);
    const auth = getAuth(app);

    // Signup
    document.getElementById("signupForm").addEventListener("submit", function(e){
      e.preventDefault();
      const email = document.getElementById("signupEmail").value;
      const password = document.getElementById("signupPassword").value;

      createUserWithEmailAndPassword(auth, email, password)
        .then((userCredential) => {
          alert("Signup successful! Welcome " + userCredential.user.email);
        })
        .catch((error) => {
          alert("Error: " + error.message);
        });
    });

    // Login
    document.getElementById("loginForm").addEventListener("submit", function(e){
      e.preventDefault();
      const email = document.getElementById("loginEmail").value;
      const password = document.getElementById("loginPassword").value;

      signInWithEmailAndPassword(auth, email, password)
        .then((userCredential) => {
          alert("Login successful! Welcome back " + userCredential.user.email);
        })
        .catch((error) => {
          alert("Error: " + error.message);
        });
    });
  </script>
</body>
</html>
