<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>VICTOR TECH STUDIO 🎥</title>
  <style>
    * {margin:0; padding:0; box-sizing:border-box;}
    body {
      font-family: Arial, sans-serif;
      background-color: #1a1a1a;
      color: #fff;
      line-height: 1.6;
    }
    header {
      background-color: #b30000;
      padding: 20px;
      text-align: center;
    }
    header h1 {
      font-size: 2.5em;
    }
    header p {
      font-size: 1.2em;
      font-style: italic;
      margin-top: 10px;
    }
    nav {
      display: flex;
      justify-content: center;
      background-color: #800000;
      padding: 10px;
      gap: 20px;
    }
    nav a {
      color: #fff;
      text-decoration: none;
      font-weight: bold;
      transition: color 0.3s;
    }
    nav a:hover {color: #ff4d4d;}
    section {
      padding: 60px 20px;
      max-width: 1000px;
      margin: auto;
    }
    section:nth-of-type(even) {background-color: #2a2a2a;}
    section h2 {
      color: #ff4d4d;
      margin-bottom: 20px;
      text-align: center;
    }
    section p {text-align: center; margin-bottom: 20px;}
    form {
      display: flex;
      flex-direction: column;
      gap: 15px;
      max-width: 500px;
      margin: auto;
    }
    input, textarea {
      padding: 10px;
      border-radius: 5px;
      border: none;
      font-size: 1em;
    }
    button {
      padding: 10px;
      border: none;
      border-radius: 5px;
      background-color: #b30000;
      color: white;
      font-weight: bold;
      cursor: pointer;
      transition: background 0.3s;
    }
    button:hover {background-color: #ff4d4d;}
    footer {
      background-color: #800000;
      text-align: center;
      padding: 20px;
      margin-top: 40px;
    }
    footer p {margin: 5px 0;}
    .logo {
      font-weight: bold;
      font-size: 2em;
      color: #fff;
      text-shadow: 2px 2px #800000;
      margin-bottom: 10px;
    }
  </style>
</head>
<body>

<header>
  <div class="logo">VICTOR TECH STUDIO 🎥</div>
  <p>We bring your memories to reality</p>
</header>

<nav>
  <a href="#home">Home</a>
  <a href="#about">About</a>
  <a href="#services">Services</a>
  <a href="#contact">Contact</a>
</nav>

<section id="home">
  <h2>Welcome to Victor Tech Studio</h2>
  <p>We specialize in bringing your memories to life through professional video production and editing.</p>
</section>

<section id="about">
  <h2>About Us</h2>
  <p>At Victor Tech Studio, we combine creativity and technology to produce stunning visuals that capture your precious moments perfectly.</p>
</section>

<section id="services">
  <h2>Our Services</h2>
  <p>Video Production | Video Editing | Photography | Event Coverage | Corporate Projects</p>
</section>

<section id="contact">
  <h2>Contact Us</h2>
  <form id="contactForm">
    <input type="text" placeholder="Your Name" required>
    <input type="email" placeholder="Your Email" required>
    <input type="text" placeholder="Phone Number" required>
    <textarea placeholder="Message" rows="5" required></textarea>
    <button type="submit">Send Message</button>
  </form>
  <p id="confirmation" style="color:#ff4d4d; font-weight:bold; text-align:center; margin-top:15px;"></p>
</section>

<footer>
  <p>Phone: 07026674472 | WhatsApp: 07058782947 | Email: moziavictor9@gmail.com</p>
  <p>Designed by Victor Mozia</p>
</footer>

<script>
  const form = document.getElementById('contactForm');
  const confirmation = document.getElementById('confirmation');

  form.addEventListener('submit', function(e){
    e.preventDefault();
    confirmation.innerText = "Thank you! Your message has been sent.";
    form.reset();
  });
</script>

</body>
</html>
