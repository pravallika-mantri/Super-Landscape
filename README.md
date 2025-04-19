<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Super Landscape - Vegan Soft Drinks</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background-color: #fff;
      color: #333;
      opacity: 0;
      animation: fadeIn 1s forwards;
    }

    @keyframes fadeIn {
      to {
        opacity: 1;
      }
    }

    header {
      background-color: #5D3FD3;
      color: white;
      padding: 2rem 4rem;
      display: flex;
      justify-content: space-between;
      align-items: center;
      box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
      border-bottom: 3px solid #4a2c8c;
      animation: slideIn 0.8s ease-out;
    }

    @keyframes slideIn {
      from {
        transform: translateY(-50px);
        opacity: 0;
      }
      to {
        transform: translateY(0);
        opacity: 1;
      }
    }

    .logo {
      display: flex;
      align-items: center;
      font-weight: bold;
    }

    .logo img {
      height: 45px;
      margin-right: 1rem;
      border-radius: 300px;
    }

    .logo h1 {
      font-size: 2rem;
      margin: 0;
    }

    nav a {
      color: white;
      margin: 0 1.5rem;
      text-decoration: none;
      font-weight: 600;
      transition: color 0.3s ease, transform 0.3s ease;
    }

    nav a:hover {
      color: #f4b744;
      transform: scale(1.1);
    }

    .hero {
      padding: 5rem 2rem;
      text-align: center;
      background-color: #f8f8f8;
      animation: heroFadeIn 1s ease-out;
    }

    @keyframes heroFadeIn {
      from {
        opacity: 0;
        transform: translateY(20px);
      }
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }

    .hero h1 {
      font-size: 3rem;
      color: #5D3FD3;
      font-weight: 700;
      margin-bottom: 1rem;
      animation: heroTitleFade 1s ease-out;
    }

    @keyframes heroTitleFade {
      from {
        opacity: 0;
        transform: translateY(20px);
      }
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }

    .hero p {
      font-size: 1.2rem;
      margin: 1rem 0;
      color: #555;
      animation: heroTextFade 1.5s ease-out;
    }

    @keyframes heroTextFade {
      from {
        opacity: 0;
        transform: translateY(20px);
      }
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }

    .cta-button {
      background-color: #5D3FD3;
      color: white;
      padding: 1rem 2rem;
      border: none;
      font-size: 1rem;
      cursor: pointer;
      border-radius: 8px;
      transition: background-color 0.3s ease, transform 0.3s ease;
    }

    .cta-button:hover {
      background-color: #4a2c8c;
      transform: scale(1.05);
    }

    .values {
      display: flex;
      justify-content: space-around;
      flex-wrap: wrap;
      padding: 3rem 1rem;
      background-color: #f8f8f8;
      animation: fadeInUp 1s ease-out;
    }

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

    .value-box {
      max-width: 250px;
      text-align: center;
      margin: 1rem;
      padding: 2rem;
      border-radius: 12px;
      background: #fff;
      box-shadow: 0 6px 15px rgba(0, 0, 0, 0.1);
      transition: transform 0.3s ease, box-shadow 0.3s ease;
    }

    .value-box:hover {
      transform: translateY(-10px);
      box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
    }

    .value-box h3 {
      color: #5D3FD3;
      font-size: 1.8rem;
      font-weight: 700;
      margin-bottom: 1rem;
    }

    .value-box p {
      font-size: 1.1rem;
      color: #666;
      line-height: 1.7;
    }

    .images-section {
      padding: 2rem 1rem;
      background-color: #fff;
      text-align: center;
      font-size: 20px;
      animation: fadeInUp 1.5s ease-out;
    }

  .drink-images {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  gap: 1.5rem;
  margin-top: 2rem;
  opacity: 0;
  animation: sectionFade 1s forwards;
  animation-delay: 0.5s;
}

@keyframes sectionFade {
  to {
    opacity: 1;
  }
}

.drink-images img {
  width: 300px;
  height: 400px;
  border-radius: 12px;
  box-shadow: 0 8px 20px rgba(0, 0, 0, 0.12);
  transition: transform 0.4s ease, box-shadow 0.4s ease;
  opacity: 0;
  transform: scale(0.9);
  animation: fadeZoomIn 0.8s forwards;
}

.drink-images img:nth-child(1) {
  animation-delay: 0.6s;
}
.drink-images img:nth-child(2) {
  animation-delay: 0.8s;
}
.drink-images img:nth-child(3) {
  animation-delay: 1s;
}
.drink-images img:nth-child(4) {
  animation-delay: 1.2s;
}

@keyframes fadeZoomIn {
  to {
    opacity: 1;
    transform: scale(1);
  }
}

.drink-images img:hover {
  transform: scale(1.05) translateY(-5px);
  box-shadow: 0 12px 25px rgba(0, 0, 0, 0.2);
}


    footer {
      text-align: center;
      padding: 2rem;
      background-color: #eee;
      font-size: 0.9rem;
      margin-top: 3rem;
    }

    @keyframes fadeIn {
      to {
        opacity: 1;
      }
    }

    @keyframes fadeSlideDown {
      from {
        opacity: 0;
        transform: translateY(-20px);
      }
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }

  </style>
</head>

<body>
  <header>
    <div class="logo">
      <img src="logo.avif" alt="Super Landscape Logo">
      <h1>Super Landscape</h1>
    </div>
    <nav>
      <a href="index.html">Home</a>
      <a href="info.html">Information</a>
      <a href="products.html">Products</a>
      <a href="privacy.html">Privacy Policy</a>
      <a href="sample.html">Get a Sample</a>
    </nav>
  </header>

  <section class="hero">
    <h1>Sip the Past. Taste the Future.</h1>
    <p>Premium vegan soft drinks served in 5-star restaurants. Created for couples, inspired by memories.</p>
    <button class="cta-button" onclick="window.location.href='sample.html'">Order a Free Sample</button>
  </section>



  <section class="images-section">
    <h2>Our Signature Flavors</h2>
    <div class="drink-images">
      <img src="img 1 .webp" alt="Berry Bliss Bottle">
      <img src="img 2.jpg" alt="Citrus Sparkle Bottle">
      <img src="img 3.jpg" alt="Classic Cola Revival">
      <img src="img 4.png" alt="Herbal Fizz">
    </div>
  </section>

  <section class="values">
    <div class="value-box">
      <h3>Nostalgia</h3>
      <p>Flavors that take you back to the best moments of your life.</p>
    </div>
    <div class="value-box">
      <h3>Elegance</h3>
      <p>Our drinks are served in the nation's finest restaurants.</p>
    </div>
    <div class="value-box">
      <h3>Conscious Living</h3>
      <p>100% vegan ingredients, crafted responsibly.</p>
    </div>
  </section>
  

  <footer>
    <p>&copy; 2025 Super Landscape. All rights reserved.</p>
  </footer>
</body>

</html>
