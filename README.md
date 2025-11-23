<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>UrbanGent - Men's Clothing</title>
    <link rel="stylesheet" href="style.css">
    <!-- Font Awesome for icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
</head>
<body>
    <!-- Header -->
    <header>
        <div class="container header-container">
            <h1>UrbanGent</h1>
            <nav>
                <ul>
                    <li><a href="#home">Home</a></li>
                    <li><a href="#about">About</a></li>
                    <li><a href="#products">Products</a></li>
                    <li><a href="#contact">Contact</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- Hero Slider -->
    <section id="home" class="hero">
        <div class="slider">
            <div class="slide active" style="background-image:url('https://via.placeholder.com/1600x600?text=Modern+Menswear');">
                <div class="slide-content">
                    <h2>Stylish Outfits for Modern Men</h2>
                    <p>Dress like a true gentleman</p>
                    <a href="#products" class="btn">Shop Now</a>
                </div>
            </div>
            <div class="slide" style="background-image:url('https://via.placeholder.com/1600x600?text=Premium+Clothing');">
                <div class="slide-content">
                    <h2>Premium Quality Fabrics</h2>
                    <p>Comfort and style combined</p>
                    <a href="#products" class="btn">Explore Collection</a>
                </div>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about">
        <div class="container">
            <h2>About UrbanGent</h2>
            <p>UrbanGent delivers premium men’s fashion with a modern edge. From casual wear to formal, find outfits that fit your style and personality.</p>
        </div>
    </section>

    <!-- Products Section -->
    <section id="products">
        <div class="container">
            <h2>Our Collection</h2>
            <div class="products-grid">
                <div class="product-card">
                    <img src="https://via.placeholder.com/300x400" alt="Product 1">
                    <h3>Classic Shirt</h3>
                    <p>$29.99</p>
                    <a href="#" class="btn">Buy Now</a>
                </div>
                <div class="product-card">
                    <img src="https://via.placeholder.com/300x400" alt="Product 2">
                    <h3>Elegant Jacket</h3>
                    <p>$79.99</p>
                    <a href="#" class="btn">Buy Now</a>
                </div>
                <div class="product-card">
                    <img src="https://via.placeholder.com/300x400" alt="Product 3">
                    <h3>Casual T-Shirt</h3>
                    <p>$19.99</p>
                    <a href="#" class="btn">Buy Now</a>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact">
        <div class="container">
            <h2>Contact Us</h2>
            <form>
                <input type="text" placeholder="Your Name" required>
                <input type="email" placeholder="Your Email" required>
                <textarea placeholder="Your Message" required></textarea>
                <button type="submit">Send Message</button>
            </form>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container footer-container">
            <p>&copy; 2025 UrbanGent. All rights reserved.</p>
            <div class="social-icons">
                <a href="#"><i class="fab fa-facebook-f"></i></a>
                <a href="#"><i class="fab fa-instagram"></i></a>
                <a href="#"><i class="fab fa-twitter"></i></a>
            </div>
        </div>
    </footer>

    <!-- Slider Script -->
    <script>
        let slides = document.querySelectorAll('.slide');
        let current = 0;

        function nextSlide() {
            slides[current].classList.remove('active');
            current = (current+1) % slides.length;
            slides[current].classList.add('active');
        }

        setInterval(nextSlide, 5000); // change slide every 5 sec
    </script>
</body>
</html>
