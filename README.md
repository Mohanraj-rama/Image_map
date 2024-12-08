# Ex04 Places Around Me
# Date:
# AIM
To develop a website to display details about the places around my house.

# DESIGN STEPS
## STEP 1
Create a Django admin interface.

## STEP 2
Download your city map from Google.

## STEP 3
Using <map> tag name the map.

## STEP 4
Create clickable regions in the image using <area> tag.

## STEP 5
Write HTML programs for all the regions identified.

## STEP 6
Execute the programs and publish them.

# CODE
### map.html
```
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>image map</title>
</head>
<body>
    <img src="imagemap2.png" usemap="#image-map">

    <map name="image-map">
        <area target="" alt="pothys" title="pothys" href="POTHYS.html" coords="414,732,444,732,437,758,421,758" shape="poly">
        <area target="" alt="saravana store" title="saravana store" href="saravanastore.html" coords="543,961,518,975,524,996,551,988,547,978" shape="poly">
        <area target="" alt="shri balaji bhavan" title="shri balaji bhavan" href="balaji.html" coords="806,449,796,468,814,484,822,464,822,457" shape="poly">
        <area target="" alt="kings of wings" title="kings of wings" href="CHINEASE.html" coords="1073,582,1086,570,1082,548,1054,548" shape="poly">
        <area target="" alt="copper kitchen" title="copper kitchen" href="copper.html" coords="818,26,820,-1,851,11,843,26" shape="poly">
    </map>
</body>
</html> 
```
### pothys.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>POTHYS</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            background-color: #f4f4f4;
        }

        header {
            background-color: #2c3e50;
            color: white;
            padding: 20px 0;
            text-align: center;
        }

        header h1 {
            margin: 0;
            font-size: 36px;
        }

        nav {
            display: flex;
            justify-content: center;
            background-color: #34495e;
        }

        nav a {
            color: white;
            padding: 14px 20px;
            text-decoration: none;
            text-align: center;
            flex: 1;
        }

        nav a:hover {
            background-color: #2980b9;
        }

        .container {
            padding: 20px;
            max-width: 1200px;
            margin: 0 auto;
        }

        .products {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
        }

        .product-card {
            border: 1px solid #ddd;
            border-radius: 8px;
            overflow: hidden;
            width: 30%;
            background-color: white;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s ease-in-out;
        }

        .product-card:hover {
            transform: scale(1.05);
        }

        .product-card img {
            width: 100%;
            height: auto;
        }

        .product-card h3 {
            padding: 10px;
            background-color: #ecf0f1;
            margin: 0;
            text-align: center;
        }

        .product-card p {
            padding: 0 10px 10px;
            text-align: center;
            font-size: 1.1em;
        }

        footer {
            background-color: #2c3e50;
            color: white;
            text-align: center;
            padding: 10px 0;
        }

        .contact-section {
            padding: 20px;
            background-color: #ecf0f1;
            border-radius: 8px;
            margin-top: 40px;
        }

        .contact-section h2 {
            text-align: center;
        }

        .contact-section p {
            text-align: center;
            font-size: 1.1em;
        }

        .footer-links {
            margin-top: 10px;
        }

        .footer-links a {
            color: white;
            margin: 0 10px;
            text-decoration: none;
        }

        .footer-links a:hover {
            text-decoration: underline;
        }

        @media (max-width: 768px) {
            .products {
                flex-direction: column;
                align-items: center;
            }

            .product-card {
                width: 80%;
            }
        }
    </style>
</head>
<body>

<header>
    <h1>POTHYS</h1>
    <p>Quality fabrics for every occasion</p>
</header>

<nav>
    <a href="#home">Home</a>
    <a href="#products">Products</a>
    <a href="#contact">Contact</a>
</nav>

<section id="home" class="container">
    <h2>Welcome to Textile Shop!</h2>
    <p>Discover a wide range of premium fabrics for all your tailoring and crafting needs. From cottons to silks, we have it all.</p>
</section>

<section id="products" class="container">
    <h2>Our Products</h2>
    <div class="products">
        <div class="product-card">
            <img src="fabriccasual.jpg" alt="Cotton Fabric">
            <h3>Cotton Fabric</h3>
            <p>Soft, breathable, and perfect for casual wear. Available in various colors and patterns.</p>
        </div>

        <div class="product-card">
            <img src="fabric.webp" alt="Silk Fabric">
            <h3>Silk Fabric</h3>
            <p>Elegant and luxurious, perfect for formal occasions and evening wear.</p>
        </div>

        <div class="product-card">
            <img src="fabricwinter.webp" alt="Wool Fabric">
            <h3>Wool Fabric</h3>
            <p>Warm and cozy, ideal for winter garments and outerwear.</p>
        </div>
    </div>
</section>

<section id="contact" class="container contact-section">
    <h2>Contact Us</h2>
    <p>If you have any questions or need assistance, feel free to get in touch with us. We are happy to help!</p>
    <p>Email: contact@textileshop.com</p>
    <p>Phone: (555) 123-4567</p>
</section>

<footer>
    <p>&copy; 2024 Textile Shop</p>
    <div class="footer-links">
        <a href="#home">Home</a>
        <a href="#products">Products</a>
        <a href="#contact">Contact</a>
    </div>
</footer>

</body>
</html>

```
### saravanastore.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Jewellery Shop</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            background-color: #f8f8f8;
        }

        header {
            background-color: #2c3e50;
            color: white;
            padding: 20px 0;
            text-align: center;
        }

        header h1 {
            margin: 0;
            font-size: 36px;
        }

        nav {
            display: flex;
            justify-content: center;
            background-color: #34495e;
        }

        nav a {
            color: white;
            padding: 14px 20px;
            text-decoration: none;
            text-align: center;
            flex: 1;
        }

        nav a:hover {
            background-color: #2980b9;
        }

        .container {
            padding: 20px;
            max-width: 1200px;
            margin: 0 auto;
        }

        .products {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
        }

        .product-card {
            border: 1px solid #ddd;
            border-radius: 8px;
            overflow: hidden;
            width: 30%;
            background-color: white;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s ease-in-out;
        }

        .product-card:hover {
            transform: scale(1.05);
        }

        .product-card img {
            width: 100%;
            height: auto;
        }

        .product-card h3 {
            padding: 10px;
            background-color: #ecf0f1;
            margin: 0;
            text-align: center;
        }

        .product-card p {
            padding: 0 10px 10px;
            text-align: center;
            font-size: 1.1em;
        }

        footer {
            background-color: #2c3e50;
            color: white;
            text-align: center;
            padding: 10px 0;
        }

        .contact-section {
            padding: 20px;
            background-color: #ecf0f1;
            border-radius: 8px;
            margin-top: 40px;
        }

        .contact-section h2 {
            text-align: center;
        }

        .contact-section p {
            text-align: center;
            font-size: 1.1em;
        }

        .footer-links {
            margin-top: 10px;
        }

        .footer-links a {
            color: white;
            margin: 0 10px;
            text-decoration: none;
        }

        .footer-links a:hover {
            text-decoration: underline;
        }

        @media (max-width: 768px) {
            .products {
                flex-direction: column;
                align-items: center;
            }

            .product-card {
                width: 80%;
            }
        }
    </style>
</head>
<body>

<header>
    <h1>Jewellery Shop</h1>
    <p>Discover our exclusive collection of handcrafted jewellery</p>
</header>

<nav>
    <a href="#home">Home</a>
    <a href="#products">Products</a>
    <a href="#contact">Contact</a>
</nav>

<section id="home" class="container">
    <h2>Welcome to Our Jewellery Shop!</h2>
    <p>We specialize in high-quality, handcrafted jewellery pieces that are designed to suit all occasions. Whether you're looking for engagement rings, necklaces, bracelets, or earrings, we have something special just for you!</p>
</section>

<section id="products" class="container">
    <h2>Our Jewellery Collection</h2>
    <div class="products">
        <div class="product-card">
            <img src="ring.webp" alt="Gold Ring">
            <h3>Gold Ring</h3>
            <p>A beautifully crafted 18K gold ring, perfect for any occasion. Elegant and timeless.</p>
        </div>

        <div class="product-card">
            <img src="neck.jpg" alt="Diamond Necklace">
            <h3>Diamond Necklace</h3>
            <p>Our stunning diamond necklace features brilliant-cut diamonds set in 14K white gold.</p>
        </div>

        <div class="product-card">
            <img src="brace.webp" alt="Silver Bracelet">
            <h3>Silver Bracelet</h3>
            <p>Elegantly designed silver bracelet, lightweight and perfect for everyday wear.</p>
        </div>
    </div>
</section>

<section id="contact" class="container contact-section">
    <h2>Contact Us</h2>
    <p>If you have any questions or need assistance with our products, feel free to reach out to us. We're here to help!</p>
    <p>Email: contact@jewelleryshop.com</p>
    <p>Phone: (555) 987-6543</p>
</section>

<footer>
    <p>&copy; 2024 Jewellery Shop</p>
    <div class="footer-links">
        <a href="#home">Home</a>
        <a href="#products">Products</a>
        <a href="#contact">Contact</a>
    </div>
</footer>

</body>
</html>

```
### copper.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Copper Kitchen Restaurant</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            background-color: #f7f7f7;
        }

        header {
            background-color: #c06c84;
            color: white;
            padding: 20px 0;
            text-align: center;
        }

        header h1 {
            margin: 0;
            font-size: 36px;
        }

        nav {
            display: flex;
            justify-content: center;
            background-color: #8e44ad;
        }

        nav a {
            color: white;
            padding: 14px 20px;
            text-decoration: none;
            text-align: center;
            flex: 1;
        }

        nav a:hover {
            background-color: #5e3370;
        }

        .container {
            padding: 20px;
            max-width: 1200px;
            margin: 0 auto;
        }

        .products {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
        }

        .product-card {
            border: 1px solid #ddd;
            border-radius: 8px;
            overflow: hidden;
            width: 30%;
            background-color: white;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s ease-in-out;
        }

        .product-card:hover {
            transform: scale(1.05);
        }

        .product-card img {
            width: 100%;
            height: auto;
        }

        .product-card h3 {
            padding: 10px;
            background-color: #ecf0f1;
            margin: 0;
            text-align: center;
        }

        .product-card p {
            padding: 0 10px 10px;
            text-align: center;
            font-size: 1.1em;
        }

        footer {
            background-color: #c06c84;
            color: white;
            text-align: center;
            padding: 10px 0;
        }

        .contact-section {
            padding: 20px;
            background-color: #ecf0f1;
            border-radius: 8px;
            margin-top: 40px;
        }

        .contact-section h2 {
            text-align: center;
        }

        .contact-section p {
            text-align: center;
            font-size: 1.1em;
        }

        .footer-links {
            margin-top: 10px;
        }

        .footer-links a {
            color: white;
            margin: 0 10px;
            text-decoration: none;
        }

        .footer-links a:hover {
            text-decoration: underline;
        }

        @media (max-width: 768px) {
            .products {
                flex-direction: column;
                align-items: center;
            }

            .product-card {
                width: 80%;
            }
        }
    </style>
</head>
<body>

<header>
    <h1>Copper Kitchen Restaurant</h1>
    <p>Experience the finest culinary delights made with love and copper cookware</p>
</header>

<nav>
    <a href="#home">Home</a>
    <a href="#menu">Menu</a>
    <a href="#contact">Contact</a>
</nav>

<section id="home" class="container">
    <h2>Welcome to Copper Kitchen</h2>
    <p>At Copper Kitchen, we believe in creating an unforgettable dining experience. Our chefs use the finest ingredients, and our signature copper cookware enhances the flavors, making every dish a masterpiece.</p>
</section>

<section id="menu" class="container">
    <h2>Our Delicious Menu</h2>
    <div class="products">
        <div class="product-card">
            <img src="gril.jpg" alt="Grilled Chicken">
            <h3>Grilled Chicken</h3>
            <p>Juicy, tender grilled chicken served with a side of crispy vegetables and a tangy sauce.</p>
        </div>

        <div class="product-card">
            <img src="vegetablecurry.jpg" alt="Vegetable Curry">
            <h3>Vegetable Curry</h3>
            <p>A rich and flavorful curry made with fresh vegetables and a blend of aromatic spices.</p>
        </div>

        <div class="product-card">
            <img src="chocoloate.webp" alt="Chocolate Mousse">
            <h3>Chocolate Mousse</h3>
            <p>A silky, creamy dessert made with the finest dark chocolate and topped with whipped cream.</p>
        </div>
    </div>
</section>

<section id="contact" class="container contact-section">
    <h2>Contact Us</h2>
    <p>Have a question or want to make a reservation? Get in touch with us, and we'll be happy to assist you!</p>
    <p>Email: contact@copperkitchen.com</p>
    <p>Phone: (555) 123-4567</p>
    <p>Address: 123 Copper Lane, Foodtown, FL 98765</p>
</section>

<footer>
    <p>&copy; 2024 Copper Kitchen Restaurant</p>
    <div class="footer-links">
        <a href="#home">Home</a>
        <a href="#menu">Menu</a>
        <a href="#contact">Contact</a>
    </div>
</footer>

</body>
</html>

```
### CHINEASE.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Chinese Delight Restaurant</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            background-color: #f9f9f9;
        }

        header {
            background-color: #ff5722;
            color: white;
            padding: 20px 0;
            text-align: center;
        }

        header h1 {
            margin: 0;
            font-size: 36px;
        }

        header p {
            font-size: 18px;
        }

        nav {
            display: flex;
            justify-content: center;
            background-color: #ff7043;
        }

        nav a {
            color: white;
            padding: 14px 20px;
            text-decoration: none;
            text-align: center;
            flex: 1;
        }

        nav a:hover {
            background-color: #f4511e;
        }

        .container {
            padding: 20px;
            max-width: 1200px;
            margin: 0 auto;
        }

        .menu {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
        }

        .menu-item {
            border: 1px solid #ddd;
            border-radius: 8px;
            overflow: hidden;
            width: 30%;
            background-color: white;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s ease-in-out;
        }

        .menu-item:hover {
            transform: scale(1.05);
        }

        .menu-item img {
            width: 100%;
            height: auto;
        }

        .menu-item h3 {
            padding: 10px;
            background-color: #ffccbc;
            margin: 0;
            text-align: center;
        }

        .menu-item p {
            padding: 0 10px 10px;
            text-align: center;
            font-size: 1.1em;
        }

        footer {
            background-color: #ff5722;
            color: white;
            text-align: center;
            padding: 10px 0;
        }

        .contact-section {
            padding: 20px;
            background-color: #ffe0b2;
            border-radius: 8px;
            margin-top: 40px;
        }

        .contact-section h2 {
            text-align: center;
        }

        .contact-section p {
            text-align: center;
            font-size: 1.1em;
        }

        .footer-links {
            margin-top: 10px;
        }

        .footer-links a {
            color: white;
            margin: 0 10px;
            text-decoration: none;
        }

        .footer-links a:hover {
            text-decoration: underline;
        }

        @media (max-width: 768px) {
            .menu {
                flex-direction: column;
                align-items: center;
            }

            .menu-item {
                width: 80%;
            }
        }
    </style>
</head>
<body>

<header>
    <h1>Chinese Delight Restaurant</h1>
    <p>Authentic Chinese Cuisine with a Modern Twist</p>
</header>

<nav>
    <a href="#home">Home</a>
    <a href="#menu">Menu</a>
    <a href="#contact">Contact</a>
</nav>

<section id="home" class="container">
    <h2>Welcome to Chinese Delight!</h2>
    <p>Chinese Delight brings the rich and varied flavors of authentic Chinese cuisine right to your table. From fresh dim sum to sizzling stir-fries, our restaurant offers a wide range of delicious dishes prepared using traditional techniques and fresh ingredients.</p>
</section>

<section id="menu" class="container">
    <h2>Our Menu</h2>
    <div class="menu">
        <div class="menu-item">
            <img src="chicken.jpg" alt="Sweet and Sour Chicken">
            <h3>Sweet and Sour Chicken</h3>
            <p>Crispy chicken pieces coated with a tangy, sweet and sour sauce, served with vegetables.</p>
        </div>

        <div class="menu-item">
            <img src="kung pao.jpg" alt="Kung Pao Chicken">
            <h3>Kung Pao Chicken</h3>
            <p>Stir-fried chicken with peanuts, bell peppers, and a savory sauce made with soy, garlic, and chili.</p>
        </div>

        <div class="menu-item">
            <img src="fried.jpg" alt="Vegetable Fried Rice">
            <h3>Vegetable Fried Rice</h3>
            <p>Aromatic fried rice with mixed vegetables, soy sauce, and a hint of ginger and garlic.</p>
        </div>
    </div>
</section>

<section id="contact" class="container contact-section">
    <h2>Contact Us</h2>
    <p>If you have any questions or would like to make a reservation, feel free to contact us. We look forward to serving you!</p>
    <p>Email: contact@chinesedelight.com</p>
    <p>Phone: (555) 123-4567</p>
    <p>Address: 123 Oriental Avenue, Food City, FC 67890</p>
</section>

<footer>
    <p>&copy; 2024 Chinese Delight Restaurant</p>
    <div class="footer-links">
        <a href="#home">Home</a>
        <a href="#menu">Menu</a>
        <a href="#contact">Contact</a>
    </div>
</footer>

</body>
</html>

```
### balaji.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Sri Balaji Bhavan Veg Restaurant</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            background-color: #f8f8f8;
        }

        header {
            background-color: #2e8b57;
            color: white;
            padding: 20px 0;
            text-align: center;
        }

        header h1 {
            margin: 0;
            font-size: 36px;
        }

        nav {
            display: flex;
            justify-content: center;
            background-color: #4CAF50;
        }

        nav a {
            color: white;
            padding: 14px 20px;
            text-decoration: none;
            text-align: center;
            flex: 1;
        }

        nav a:hover {
            background-color: #45a049;
        }

        .container {
            padding: 20px;
            max-width: 1200px;
            margin: 0 auto;
        }

        .menu {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
        }

        .menu-item {
            border: 1px solid #ddd;
            border-radius: 8px;
            overflow: hidden;
            width: 30%;
            background-color: white;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s ease-in-out;
        }

        .menu-item:hover {
            transform: scale(1.05);
        }

        .menu-item img {
            width: 100%;
            height: auto;
        }

        .menu-item h3 {
            padding: 10px;
            background-color: #f1f1f1;
            margin: 0;
            text-align: center;
        }

        .menu-item p {
            padding: 0 10px 10px;
            text-align: center;
            font-size: 1.1em;
        }

        footer {
            background-color: #2e8b57;
            color: white;
            text-align: center;
            padding: 10px 0;
        }

        .contact-section {
            padding: 20px;
            background-color: #f1f1f1;
            border-radius: 8px;
            margin-top: 40px;
        }

        .contact-section h2 {
            text-align: center;
        }

        .contact-section p {
            text-align: center;
            font-size: 1.1em;
        }

        .footer-links {
            margin-top: 10px;
        }

        .footer-links a {
            color: white;
            margin: 0 10px;
            text-decoration: none;
        }

        .footer-links a:hover {
            text-decoration: underline;
        }

        @media (max-width: 768px) {
            .menu {
                flex-direction: column;
                align-items: center;
            }

            .menu-item {
                width: 80%;
            }
        }
    </style>
</head>
<body>

<header>
    <h1>Sri Balaji Bhavan Veg Restaurant</h1>
    <p>Serving Authentic South Indian Vegetarian Cuisine</p>
</header>

<nav>
    <a href="#home">Home</a>
    <a href="#menu">Menu</a>
    <a href="#contact">Contact</a>
</nav>

<section id="home" class="container">
    <h2>Welcome to Sri Balaji Bhavan!</h2>
    <p>At Sri Balaji Bhavan, we offer a wide range of authentic vegetarian dishes made with the finest ingredients. Our menu features traditional South Indian delicacies prepared with love and care to deliver the perfect meal experience.</p>
</section>

<section id="menu" class="container">
    <h2>Our Menu</h2>
    <div class="menu">
        <div class="menu-item">
            <img src="masala.jpg" alt="Masala Dosa">
            <h3>Masala Dosa</h3>
            <p>Thin, crispy dosa stuffed with a spicy potato filling, served with chutneys and sambar.</p>
        </div>

        <div class="menu-item">
            <img src="idli.webp" alt="Idli Sambar">
            <h3>Idli Sambar</h3>
            <p>Soft, steamed rice cakes served with spicy sambar and coconut chutney.</p>
        </div>

        <div class="menu-item">
            <img src="veg birinji.webp" alt="Vegetable Biryani">
            <h3>Vegetable Biryani</h3>
            <p>Aromatic basmati rice cooked with mixed vegetables and spices, served with raita.</p>
        </div>
    </div>
</section>

<section id="contact" class="container contact-section">
    <h2>Contact Us</h2>
    <p>If you have any questions or would like to make a reservation, feel free to get in touch with us!</p>
    <p>Email: contact@balajibhavan.com</p>
    <p>Phone: (555) 987-6543</p>
    <p>Address: 456 South Indian Street, Veg City, VC 12345</p>
</section>

<footer>
    <p>&copy; 2024 Sri Balaji Bhavan Veg Restaurant</p>
    <div class="footer-links">
        <a href="#home">Home</a>
        <a href="#menu">Menu</a>
        <a href="#contact">Contact</a>
    </div>
</footer>

</body>
</html>

```
# OUTPUT
![alt text](<Screenshot (38).png>)
![alt text](<Screenshot (39).png>)
![alt text](<Screenshot (44).png>)
![alt text](<Screenshot (43).png>)
![alt text](<Screenshot (42).png>)
![alt text](<Screenshot (41).png>)
# RESULT
The program for implementing image maps using HTML is executed successfully.
