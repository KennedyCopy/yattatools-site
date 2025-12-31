# yattatools-site
YattaTools hardware website
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>YattaTools (YT) - Premium Hardware Tools</title>
    <meta name="description" content="YattaTools (YT) - Your go-to source for reliable power tools, hand tools, and hardware accessories.">
    <style>
        /* Reset and Basics */
        * { margin: 0; padding: 0; box-sizing: border-box; }
        body { font-family: 'Arial', sans-serif; line-height: 1.6; color: #333; background: #f4f4f4; }
        a { text-decoration: none; color: inherit; }
        img { max-width: 100%; height: auto; display: block; }
        
        /* Colors: Orange/Black for hardware vibe */
        :root { --primary: #ff6600; --dark: #222; --light: #fff; }
        
        /* Header */
        header { background: var(--dark); color: var(--light); padding: 1rem; position: fixed; width: 100%; top: 0; z-index: 1000; box-shadow: 0 2px 10px rgba(0,0,0,0.2); }
        .nav-container { display: flex; justify-content: space-between; align-items: center; max-width: 1200px; margin: 0 auto; }
        .logo { font-size: 1.8rem; font-weight: bold; }
        .logo span { color: var(--primary); }
        nav ul { display: flex; list-style: none; }
        nav ul li { margin-left: 2rem; }
        nav ul li a { font-weight: bold; transition: color 0.3s; }
        nav ul li a:hover { color: var(--primary); }
        .menu-toggle { display: none; font-size: 1.5rem; cursor: pointer; }
        
        /* Hero */
        .hero { background: linear-gradient(rgba(0,0,0,0.6), rgba(0,0,0,0.6)), url('https://media.istockphoto.com/id/1077311966/photo/wooden-background-with-a-tools-banner-for-a-hardware-store-and-a-building-company.jpg?s=612x612&w=0&k=20&c=7XZ0DxRdRPfy7LR2CA9FUoAIq9lh9chfTH0OdgXsIwE=') center/cover no-repeat; height: 100vh; display: flex; align-items: center; justify-content: center; text-align: center; color: var(--light); margin-top: 70px; }
        .hero-content h1 { font-size: 3.5rem; margin-bottom: 1rem; }
        .hero-content p { font-size: 1.5rem; margin-bottom: 2rem; }
        .btn { background: var(--primary); color: var(--light); padding: 1rem 2rem; border-radius: 5px; font-weight: bold; transition: background 0.3s; }
        .btn:hover { background: #e65c00; }
        
        /* Sections */
        section { padding: 4rem 2rem; max-width: 1200px; margin: 0 auto; }
        h2 { text-align: center; font-size: 2.5rem; margin-bottom: 2rem; color: var(--dark); }
        .products-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 2rem; }
        .product-card { background: var(--light); border-radius: 10px; overflow: hidden; box-shadow: 0 5px 15px rgba(0,0,0,0.1); text-align: center; transition: transform 0.3s; }
        .product-card:hover { transform: translateY(-10px); }
        .product-card img { width: 100%; height: 250px; object-fit: cover; }
        .product-info { padding: 1.5rem; }
        .product-info h3 { margin-bottom: 0.5rem; }
        .price { font-size: 1.5rem; color: var(--primary); font-weight: bold; margin: 1rem 0; }
        
        /* About */
        .about { background: #eee; }
        
        /* Footer */
        footer { background: var(--dark); color: var(--light); text-align: center; padding: 2rem; }
        
        /* Responsive */
        @media (max-width: 768px) {
            .menu-toggle { display: block; }
            nav ul { display: none; flex-direction: column; position: absolute; top: 100%; left: 0; width: 100%; background: var(--dark); }
            nav ul.active { display: flex; }
            nav ul li { margin: 1rem 0; text-align: center; }
            .hero-content h1 { font-size: 2.5rem; }
        }
    </style>
</head>
<body>
    <header>
        <div class="nav-container">
            <div class="logo">Yatta<span>Tools</span> (YT)</div>
            <nav>
                <div class="menu-toggle" onclick="toggleMenu()">☰</div>
                <ul id="nav-menu">
                    <li><a href="#home">Home</a></li>
                    <li><a href="#products">Products</a></li>
                    <li><a href="#about">About</a></li>
                    <li><a href="#contact">Contact</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <section id="home" class="hero">
        <div class="hero-content">
            <h1>YattaTools (YT)</h1>
            <p>Power Up Your Projects with Premium Hardware Tools</p>
            <a href="#products" class="btn">Shop Now</a>
        </div>
    </section>

    <section id="products">
        <h2>Featured Tools</h2>
        <div class="products-grid">
            <div class="product-card">
                <img src="https://cdn.thewirecutter.com/wp-content/media/2020/12/powerdrills-2048px-0781.jpg?auto=webp&quality=75&crop=1.91:1&width=1200" alt="Cordless Power Drill">
                <div class="product-info">
                    <h3>Cordless Power Drill</h3>
                    <p>High-torque drill for heavy-duty jobs.</p>
                    <div class="price">$129.99</div>
                    <a href="#" class="btn">Add to Cart</a>
                </div>
            </div>
            <div class="product-card">
                <img src="https://cdn.thewirecutter.com/wp-content/media/2025/05/BEST-DRILLS-2048px-3209.jpg?auto=webp&quality=75&width=1024" alt="Professional Drill Set">
                <div class="product-info">
                    <h3>Professional Drill Kit</h3>
                    <p>Complete set with bits and battery.</p>
                    <div class="price">$199.99</div>
                    <a href="#" class="btn">Add to Cart</a>
                </div>
            </div>
            <div class="product-card">
                <img src="https://m.media-amazon.com/images/I/5164LCmfiPL._AC_UF894,1000_QL80_.jpg" alt="Hammer & Screwdriver Set">
                <div class="product-info">
                    <h3>Hammer & Screwdriver Set</h3>
                    <p>Essential hand tools for every toolbox.</p>
                    <div class="price">$49.99</div>
                    <a href="#" class="btn">Add to Cart</a>
                </div>
            </div>
            <!-- Add more products here -->
        </div>
    </section>

    <section id="about" class="about">
        <h2>About YattaTools</h2>
        <p style="max-width: 800px; margin: 0 auto; text-align: center;">YattaTools (YT) is dedicated to providing high-quality hardware tools for DIY enthusiasts, professionals, and contractors. From power drills to hand tools, we source reliable products to help you tackle any project with confidence.</p>
    </section>

    <footer id="contact">
        <p>&copy; 2025 YattaTools (YT). All rights reserved.</p>
        <p>Email: info@yattatools.com | Phone: (123) 456-7890</p>
    </footer>

    <script>
        function toggleMenu() {
            document.getElementById('nav-menu').classList.toggle('active');
        }
    </script>
</body>
</html>
