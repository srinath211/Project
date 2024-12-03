<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Simple E-Commerce Website</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        /* Body and general layout */
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            color: #333;
            margin: 0;
        }
        
        /* Header Styling */
        header {
            background-color: #333;
            color: white;
            padding: 20px;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        header .logo h1 {
            font-size: 30px;
            font-weight: bold;
        }
        
        header nav ul {
            list-style-type: none;
            display: flex;
        }
        
        header nav ul li {
            margin-left: 20px;
        }
        
        header nav ul li a {
            color: white;
            text-decoration: none;
            font-size: 18px;
        }
        
        /* Main Content Section */
        main {
            padding: 20px;
            text-align: center;
        }
        
        main h2 {
            font-size: 28px;
            margin-bottom: 20px;
        }
        
        /* Product Listing Styles */
        .products {
            display: flex;
            justify-content: space-around;
            flex-wrap: wrap;
            gap: 20px;
        }
        
        .product {
            background-color: white;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            width: 200px;
            text-align: center;
            padding: 15px;
            transition: transform 0.2s;
        }
        
        .product img {
            width: 100%;
            border-radius: 8px;
        }
        
        .product h3 {
            margin-top: 15px;
            font-size: 20px;
        }
        
        .product p {
            font-size: 18px;
            color: #555;
            margin-bottom: 15px;
        }
        
        .product button {
            background-color: #333;
            color: white;
            border: none;
            padding: 10px;
            cursor: pointer;
            width: 100%;
            border-radius: 4px;
        }
        
        .product button:hover {
            background-color: #555;
        }
        
        .product:hover {
            transform: translateY(-10px);
        }
        
        /* Footer Styling */
        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 10px;
            position: fixed;
            bottom: 0;
            width: 100%;
        }
        
        /* Cart Icon Styling */
        #cart-count {
            background-color: red;
            color: white;
            border-radius: 50%;
            padding: 5px 10px;
            font-size: 16px;
        }
        </style>
</head>
<body>
    <!-- Header Section -->
    <header>
        <div class="logo">
            <h1>ShopEase</h1>
        </div>
        <nav>
            <ul>
                <li><a href="#">Home</a></li>
                <li><a href="#">Shop</a></li>
                <li><a href="#">Contact</a></li>
                <li><a href="#">Cart <span id="cart-count">0</span></a></li>
            </ul>
        </nav>
    </header>

    <!-- Main Content Section -->
    <main>
        <h2>Our Products</h2>
        <div class="products">
            <div class="product">
                <img src="https://encrypted-tbn0.gstatic.com/shopping?q=tbn:ANd9GcShbEa7WnFOOMYRLZIdsiR7MB2PTKWREWCA7bP8RAqftvY5sfKg7VEQ8Xq64QZrDoI1Dnq4BHMUQKpukbUxcx3hgF2td9WLmwPYBC7340rVLWEy8BdmxLJPOZzRYBxlTQlW44i8baI&usqp=CAc" alt="Product 1">
                <h3>Product 1</h3>
                <p>$20.00</p>
                <button onclick="addToCart()">Add to Cart</button>
            </div>
            <div class="product">
                <img src="https://encrypted-tbn2.gstatic.com/shopping?q=tbn:ANd9GcSmENMCECpH18xMhpq5btTPsTjRk1xZOZFkX1ZureDwQ0HfwBn3HMx0B1qDNRF6b4RAcCBYrrGwkHXnXdUNCcsVJVOnZnCZiqH2pPvIpfwjCw-ozLLGSKgTn_4IZmHm4mBOmDEaow&usqp=CAc" alt="Product 2">
                <h3>Product 2</h3>
                <p>$30.00</p>
                <button onclick="addToCart()">Add to Cart</button>
            </div>
            <div class="product">
                <img src="https://m.media-amazon.com/images/I/715Dsu2jxWL.jpg" alt="Product 3">
                <h3>Product 3</h3>
                <p>$40.00</p>
                <button onclick="addToCart()">Add to Cart</button>
            </div>
            <div class="product">
                <img src="https://rukminim2.flixcart.com/image/850/1000/xif0q/power-bank/0/j/r/lm-pb436-battery-capacity-10000mah-2-usb-ports-4-in-1-cable-ios-original-imagk34um6npezdh.jpeg?q=20&crop=false" alt="Product 4">
                <h3>Product 4</h3>
                <p>$40.00</p>
                <button onclick="addToCart()">Add to Cart</button>
            </div>
            
        </div>
    </main>

    <!-- Footer Section -->
    <footer>
        <p>&copy; 2024 ShopEase. All rights reserved.</p>
    </footer>

    <script src="scripts.js"></script>
</body>
</html>
