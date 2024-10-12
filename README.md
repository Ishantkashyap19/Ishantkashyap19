

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="MP Birla Cement Dealer Website">
  <title>MP Birla Cement - Official Dealer</title>
  <link rel="stylesheet" href="css/style.css">
</head>
<body>
  <header>
    <div class="container">
      <img src="images/logo.png" alt="MP Birla Cement Logo" class="logo">
      <nav>
        <ul>
          <li><a href="#home">Home</a></li>
          <li><a href="#products">Products</a></li>
          <li><a href="#about">About Us</a></li>
          <li><a href="#contact">Contact</a></li>
        </ul>
      </nav>
    </div>
  </header>

  <section id="home">
    <div class="banner">
      <h1>Welcome to MP Birla Cement Dealer</h1>
      <p>Your trusted partner for all cement needs</p>
      <a href="#products" class="btn">Explore Products</a>
    </div>
  </section>

  <section id="products">
    <div class="container">
      <h2>Our Products</h2>
      <div class="product-list">
        <div class="product">
          <img src="images/product1.jpg" alt="Product 1">
          <h3>MP Birla Cement Premium</h3>
          <p>High-quality cement for construction purposes.</p>
        </div>
        <div class="product">
          <img src="images/product2.jpg" alt="Product 2">
          <h3>MP Birla Cement Ultimate</h3>
          <p>Strong, durable cement for heavy construction.</p>
        </div>
        <!-- Add more products as needed -->
      </div>
    </div>
  </section>

  <section id="about">
    <div class="container">
      <h2>About Us</h2>
      <p>We are authorized dealers of MP Birla Cement, committed to delivering high-quality cement for all your construction needs.</p>
    </div>
  </section>

  <section id="contact">
    <div class="container">
      <h2>Contact Us</h2>
      <form action="#">
        <label for="name">Name:</label>
        <input type="text" id="name" name="name" required>
        
        <label for="email">Email:</label>
        <input type="email" id="email" name="email" required>
        
        <label for="message">Message:</label>
        <textarea id="message" name="message" required></textarea>
        
        <button type="submit">Send Message</button>
      </form>
    </div>
  </section>

  <footer>
    <div class="container">
      <p>&copy; 2024 MP Birla Cement Dealer. All rights reserved.</p>
    </div>
  </footer>

  <script src="js/scripts.js"></script>
</body>
</html>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: Arial, sans-serif;
  line-height: 1.6;
}

header {
  background: #333;
  color: #fff;
  padding: 1rem 0;
}

header .container {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

header nav ul {
  display: flex;
  list-style: none;
}

header nav ul li {
  margin-left: 20px;
}

header nav ul li a {
  color: #fff;
  text-decoration: none;
}

.banner {
  background: url('../images/banner.jpg') no-repeat center center/cover;
  height: 80vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  color: #fff;
}

.banner h1 {
  font-size: 3rem;
}

.banner p {
  font-size: 1.5rem;
}

.btn {
  display: inline-block;
  background: #ff6600;
  color: #fff;
  padding: 10px 20px;
  margin-top: 20px;
  text-decoration: none;
  border-radius: 5px;
}

section {
  padding: 2rem 0;
}

.container {
  max-width: 1100px;
  margin: 0 auto;
  padding: 0 20px;
}

#products .product-list {
  display: flex;
  justify-content: space-around;
}

#products .product {
  text-align: center;
}

#products .product img {
  width: 100%;
  height: auto;
}

footer {
  background: #333;
  color: #fff;
  text-align: center;
  padding: 1rem 0;
}
document.addEventListener("DOMContentLoaded", () => {
  const form = document.querySelector('form');
  
  form.addEventListener('submit', (event) => {
    event.preventDefault();
    const name = document.getElementById('name').value;
    const email = document.getElementById('email').value;
    const message = document.getElementById('message').value;

    alert(`Thanks for contacting us, ${name}! We will respond to your message soon.`);
  });
});
