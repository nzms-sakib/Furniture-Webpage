# Furniture-Webpage
 HTML codes
 <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Edgecut - Furniture Store</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <div class="logo">EDGE<span>CUT</span></div>
        <nav>
            <ul>
                <li><a href="#">Home</a></li>
                <li><a href="#">About</a></li>
                <li><a href="#">Furnitures</a></li>
                <li><a href="#">Blog</a></li>
                <li><a href="#">Contact Us</a></li>
                <li><a href="#">Login</a></li>
            </ul>
        </nav>
    </header>
    <main>
        <section class="hero">
            <div class="hero-text">
                <h1>FOR ALL YOUR <br> FURNITURE NEEDS</h1>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                <div class="buttons">
                    <a href="#" class="btn orange">Contact Us</a>
                    <a href="#" class="btn blue">About Us</a>
                </div>
            </div>
            <div class="hero-image">
                <img src="assets/slider-img.png" alt="Furniture Image">
            </div>
        </section>
        <section class="products">
            <h2>OUR FURNITURE</h2>
            <div class="product-list">
                <div class="product">
                    <img src="assets/f1.png" alt="Brown Chair">
                    <h3>Brown Chair Design</h3>
                    <p>$100.00</p>
                    <a href="#">BUY NOW</a>
                </div>
                <div class="product">
                    <img src="assets/f2.png" alt="Double Bed">
                    <h3>Double Bed Design</h3>
                    <p>$200.00</p>
                    <a href="#">BUY NOW</a>
                </div>
                <div class="product">
                    <img src="assets/f3.png" alt="House Chair">
                    <h3>House Chair Design</h3>
                    <p>$200.00</p>
                    <a href="#">BUY NOW</a>
                </div>
                <div class="product">
                    <img src="assets/f4.png" alt="Brown Table">
                    <h3>Brown Table Design</h3>
                    <p>$100.00</p>
                    <a href="#">BUY NOW</a>
                </div>
                <div class="product">
                    <img src="assets/f5.png" alt="Blue Chair">
                    <h3>Blue Chair Design</h3>
                    <p>$200.00</p>
                    <a href="#">BUY NOW</a>
                </div>
                <div class="product">
                    <img src="assets/f6.png" alt="Mirror Table">
                    <h3>Mirror Table Design</h3>
                    <p>$200.00</p>
                    <a href="#">BUY NOW</a>
                </div>
            </div>
        </section>
        <section class="about-us">
            <div class="image">
              <img src="assets/client.jpg" alt="About Us Image">
            </div>
            <div class="text">
              <h2>About Us</h2>
              <p>We are a team of passionate individuals dedicated to making the world a better place through innovation and creativity. Our mission is to solve complex challenges and create lasting impact with our work.</p>
              <p>We believe in teamwork, dedication, and excellence. Join us on our journey and be part of something extraordinary!</p>
            </div>
          </section>
    </main>
</body>
</html>

__________________________________________________________________________________________________________________________________________________________________________________________________________________


CSS Codes
/* Global Styles */
body {
    font-family: 'Poppins', sans-serif;
    margin: 0;
    padding: 0;
    background: #f8f8f8;
    color: #333;
}

/* Header */
header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px 50px;
    background: white;
    border-bottom: 2px solid #eee;
}

.logo {
    font-size: 24px;
    font-weight: bold;
}

.logo span {
    color: #ff6600;
}

nav ul {
    list-style: none;
    display: flex;
    gap: 20px;
    padding: 0;
}

nav ul li {
    display: inline;
}

nav ul li a {
    text-decoration: none;
    color: black;
    font-weight: bold;
}

/* Hero Section */
.hero {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 50px;
    background: #f4f4f4;
}

.hero-text {
    max-width: 50%;
}

.hero-text h1 {
    font-size: 36px;
    font-weight: bold;
}

.hero .btn {
    display: inline-block;
    padding: 10px 20px;
    border-radius: 5px;
    text-decoration: none;
    color: white;
    margin-right: 10px;
    font-weight: bold;
}

.btn.orange {
    background: #ff6600;
}

.btn.blue {
    background: #007bff;
}

/* Product Section */
.products {
    text-align: center;
    padding: 50px;
}

.product-list {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 20px;
    justify-content: center;
}

.product {
    background: white;
    padding: 20px;
    text-align: center;
    border-radius: 10px;
    box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.1);
}

.product img {
    max-width: 100%;
    height: auto;
}

.product h3 {
    font-size: 18px;
    margin: 10px 0;
}

.product p {
    font-size: 16px;
    color: #007bff;
}

.product a {
    text-decoration: none;
    color: #ff6600;
    font-weight: bold;
}
.about-us {
    display: flex;
    height: 100vh;
  }
  
  .about-us .image {
    flex: 1;
    background-color: #f4f4f4;
  }
  
  .about-us .image img {
    width: 100%;
    height: 100%;
    object-fit: cover;
  }
  
  .about-us .text {
    flex: 1;
    padding: 40px;
    background-color: #ffffff;
    color: #333;
  }
  
  .about-us .text h2 {
    font-size: 2.5rem;
    margin-bottom: 20px;
  }
  
  .about-us .text p {
    font-size: 1.2rem;
    margin-bottom: 15px;
  }


/* Responsive Design */
@media (max-width: 768px) {
    .hero {
        flex-direction: column;
        text-align: center;
    }
    .hero-text {
        max-width: 100%;
    }
    .product-list {
        grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    }
}
