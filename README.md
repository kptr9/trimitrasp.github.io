<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>BuildPro Materials - Quality Construction Supplies</title>
    <style>
        :root {
            --primary: #2c3e50;
            --secondary: #e74c3c;
            --light: #ecf0f1;
            --dark: #2c3e50;
            --font-main: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: var(--font-main);
            line-height: 1.6;
            color: var(--dark);
            background-color: #f9f9f9;
        }
        
        header {
            background-color: var(--primary);
            color: white;
            padding: 1rem 0;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }
        
        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
        }
        
        .header-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .logo {
            font-size: 1.8rem;
            font-weight: bold;
            color: white;
            text-decoration: none;
        }
        
        nav ul {
            display: flex;
            list-style: none;
        }
        
        nav ul li {
            margin-left: 1.5rem;
        }
        
        nav ul li a {
            color: white;
            text-decoration: none;
            font-weight: 500;
            transition: color 0.3s;
        }
        
        nav ul li a:hover {
            color: var(--secondary);
        }
        
        .hero {
            background: linear-gradient(rgba(0,0,0,0.6), rgba(0,0,0,0.6)), url('https://images.unsplash.com/photo-1600585154340-be6161a56a0c?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80');
            background-size: cover;
            background-position: center;
            color: white;
            text-align: center;
            padding: 5rem 1rem;
        }
        
        .hero h1 {
            font-size: 2.5rem;
            margin-bottom: 1rem;
        }
        
        .hero p {
            font-size: 1.2rem;
            max-width: 700px;
            margin: 0 auto 2rem;
        }
        
        .btn {
            display: inline-block;
            background-color: var(--secondary);
            color: white;
            padding: 0.8rem 1.5rem;
            border-radius: 4px;
            text-decoration: none;
            font-weight: bold;
            transition: background-color 0.3s;
        }
        
        .btn:hover {
            background-color: #c0392b;
        }
        
        .products {
            padding: 4rem 0;
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 3rem;
            font-size: 2rem;
            color: var(--primary);
        }
        
        .product-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
            gap: 2rem;
        }
        
        .product-card {
            background-color: white;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 3px 10px rgba(0,0,0,0.1);
            transition: transform 0.3s;
        }
        
        .product-card:hover {
            transform: translateY(-5px);
        }
        
        .product-img {
            height: 200px;
            overflow: hidden;
        }
        
        .product-img img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.5s;
        }
        
        .product-card:hover .product-img img {
            transform: scale(1.05);
        }
        
        .product-info {
            padding: 1.5rem;
        }
        
        .product-info h3 {
            margin-bottom: 0.5rem;
            font-size: 1.2rem;
        }
        
        .product-info p {
            color: #666;
            margin-bottom: 1rem;
        }
        
        .price {
            font-weight: bold;
            color: var(--secondary);
            font-size: 1.2rem;
        }
        
        footer {
            background-color: var(--dark);
            color: white;
            text-align: center;
            padding: 2rem 0;
            margin-top: 2rem;
        }
        
        .footer-content {
            display: flex;
            justify-content: space-around;
            flex-wrap: wrap;
            margin-bottom: 1.5rem;
        }
        
        .footer-section {
            flex: 1;
            min-width: 250px;
            margin-bottom: 1rem;
            padding: 0 1rem;
        }
        
        .footer-section h3 {
            margin-bottom: 1rem;
            font-size: 1.2rem;
        }
        
        .footer-section ul {
            list-style: none;
        }
        
        .footer-section ul li {
            margin-bottom: 0.5rem;
        }
        
        .footer-section ul li a {
            color: #bbb;
            text-decoration: none;
            transition: color 0.3s;
        }
        
        .footer-section ul li a:hover {
            color: white;
        }
        
        .copyright {
            border-top: 1px solid #444;
            padding-top: 1rem;
            font-size: 0.9rem;
            color: #bbb;
        }
        
        @media (max-width: 768px) {
            .header-content {
                flex-direction: column;
                text-align: center;
            }
            
            nav ul {
                margin-top: 1rem;
                justify-content: center;
            }
            
            nav ul li {
                margin: 0 0.75rem;
            }
            
            .hero h1 {
                font-size: 2rem;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="container header-content">
            <a href="#" class="logo">BuildPro</a>
            <nav>
                <ul>
                    <li><a href="#">Home</a></li>
                    <li><a href="#products">Products</a></li>
                    <li><a href="#">About</a></li>
                    <li><a href="#">Contact</a></li>
                </ul>
            </nav>
        </div>
    </header>
    
    <section class="hero">
        <div class="container">
            <h1>Quality Building Materials for Professionals & DIYers</h1>
            <p>We supply premium construction materials at competitive prices with nationwide delivery options.</p>
            <a href="#products" class="btn">View Products</a>
        </div>
    </section>
    
    <section id="products" class="products">
        <div class="container">
            <h2 class="section-title">Our Products</h2>
            <div class="product-grid">
                <div class="product-card">
                    <div class="product-img">
                        <img src="https://images.unsplash.com/photo-1605100804763-247f67b3557e?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80" alt="Cement Bags">
                    </div>
                    <div class="product-info">
                        <h3>Premium Cement</h3>
                        <p>High-quality Portland cement for all construction needs</p>
                        <div class="price">$8.99/bag</div>
                    </div>
                </div>
                
                <div class="product-card">
                    <div class="product-img">
                        <img src="https://images.unsplash.com/photo-1600585152220-90363fe7e115?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80" alt="Bricks">
                    </div>
                    <div class="product-info">
                        <h3>Clay Bricks</h3>
                        <p>Durable red clay bricks for walls and structures</p>
                        <div class="price">$0.75/brick</div>
                    </div>
                </div>
                
                <div class="product-card">
                    <div class="product-img">
                        <img src="https://images.unsplash.com/photo-1605152276897-4f618f831968?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80" alt="Sand">
                    </div>
                    <div class="product-info">
                        <h3>Construction Sand</h3>
                        <p>Washed river sand for concrete and masonry work</p>
                        <div class="price">$45/ton</div>
                    </div>
                </div>
                
                <div class="product-card">
                    <div class="product-img">
                        <img src="https://images.unsplash.com/photo-1597852074816-d933c7d2b988?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80" alt="Steel Rods">
                    </div>
                    <div class="product-info">
                        <h3>Steel Reinforcement Rods</h3>
                        <p>High-tensile steel rebars for concrete reinforcement</p>
                        <div class="price">$0.95/lb</div>
                    </div>
                </div>
                
                <div class="product-card">
                    <div class="product-img">
                        <img src="https://images.unsplash.com/photo-1602744846299-50a5334d0b95?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80" alt="Roofing">
                    </div>
                    <div class="product-info">
                        <h3>Roofing Materials</h3>
                        <p>Various roofing options including shingles and metal</p>
                        <div class="price">From $1.50/sq.ft</div>
                    </div>
                </div>
                
                <div class="product-card">
                    <div class="product-img">
                        <img src="https://images.unsplash.com/photo-1556910639-1cf8eed3037f?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80" alt="Pipes">
                    </div>
                    <div class="product-info">
                        <h3>PVC Pipes</h3>
                        <p>Durable plumbing pipes in various diameters</p>
                        <div class="price">From $3.50/ft</div>
                    </div>
                </div>
            </div>
        </div>
    </section>
    
    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="footer-section">
                    <h3>Quick Links</h3>
                    <ul>
                        <li><a href="#">Home</a></li>
                        <li><a href="#products">Products</a></li>
                        <li><a href="#">About Us</a></li>
                        <li><a href="#">Contact</a></li>
                    </ul>
                </div>
                
                <div class="footer-section">
                    <h3>Products</h3>
                    <ul>
                        <li><a href="#">Cement & Concrete</a></li>
                        <li><a href="#">Bricks & Blocks</a></li>
                        <li><a href="#">Steel & Metal</a></li>
                        <li><a href="#">Plumbing</a></li>
                    </ul>
                </div>
                
                <div class="footer-section">
                    <h3>Contact Us</h3>
                    <ul>
                        <li>123 Construction Street</li>
                        <li>Build City, BC 12345</li>
                        <li>Phone: (555) 123-4567</li>
                        <li>Email: info@buildpro.com</li>
                    </ul>
                </div>
            </div>
            
            <div class="copyright">
                <p>&copy; 2023 BuildPro Materials. All rights reserved.</p>
            </div>
        </div>
    </footer>
</body>
</html>
