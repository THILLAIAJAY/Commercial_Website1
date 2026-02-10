# Ex02 Commercial Website
## Date: 02-02-2026
## Name: Thillai Ajay L
## Reg No: 212224040354
## AIM
To create a commercial website using CSS Flexbox.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for Homepage, Products / Services, About Us, Contact Details and User Account.

### STEP 5
Include social media links at the footer with copyright information.

### STEP 6
Define global styles for fonts, colors, and layout.

### STEP 7
Style the header, navigation bar, and sections.

### STEP 8
Use Flexbox for layout design.

### STEP 9
Add hover effects and transitions for interactivity.

### STEP 10
Add Images and Media.

### STEP 11
Use optimized images for a professional look.

### STEP 12
Open the HTML file in a browser to check layout and functionality.

### STEP 13
Fix styling issues and refine content placement.

### STEP 14
Deploy the website.

### STEP 15
Upload to GitHub Pages for free hosting.

## PROGRAM
Index.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Commercial Website</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

<header>
    <h1 >DMart</h1>
    <nav>
        <a href="#home">Home</a>
        <a href="#products">Products</a>
        <a href="#about">About Us</a>
        <a href="#contact">Contact</a>
        <a href="#account">Account</a>
    </nav>
</header>

<section id="home" class="section">
    <h2>Welcome to DMart</h2>
    <p>Your one-stop shop for quality products.</p>
</section>
<section id="products" class="section flex-container">

    <a href="#groceries" class="card-link">
        <div class="card">
            <img src="images/groceries.jpg" alt="Groceries">
            <h3>Groceries</h3>
            <ul>
                <li>Rice & Grains</li>
                <li>Vegetables</li>
                <li>Fruits</li>
                <li>Snacks</li>
            </ul>
        </div>
    </a>

    <a href="#electronics" class="card-link">
        <div class="card">
            <img src="images/electronics.jpeg" alt="Electronics">
            <h3>Electronics</h3>
            <ul>
                <li>TV</li>
                <li>Washing Machine</li>
                <li>Mixer Grinder</li>
                <li>Accessories</li>
            </ul>
        </div>
    </a>

    <a href="#dresses" class="card-link">
        <div class="card">
            <img src="images/dresses.jpeg" alt="Dresses">
            <h3>Dresses</h3>
            <ul>
                <li>Men Wear</li>
                <li>Women Wear</li>
                <li>Kids Wear</li>
                <li>Footwear</li>
            </ul>
        </div>
    </a>

</section>


<section id="about" class="section">
    <h2>About Us</h2>
    <p>DMart is a modern commercial website built using CSS Flexbox.</p>
</section>
<section id="groceries" class="section">
    <h2>Groceries Section</h2>
    <p>
        DMart offers a wide range of groceries including fresh food items and
        daily household essentials at affordable prices.
    </p>

    <ul>
        <li>Rice, wheat, pulses and grains</li>
        <li>Fresh vegetables and seasonal fruits</li>
        <li>Cooking oils, spices and condiments</li>
        <li>Snacks, biscuits and packaged food</li>
        <li>Beverages and dairy products</li>
    </ul>
</section>

<section id="electronics" class="section">
    <h2>Electronics Section</h2>
    <p>
        The electronics section provides quality home appliances and accessories
        designed to make daily life easier and more comfortable.
    </p>

    <ul>
        <li>Televisions and home entertainment systems</li>
        <li>Washing machines and refrigerators</li>
        <li>Mixer grinders and kitchen appliances</li>
        <li>Fans, irons and electrical accessories</li>
        <li>Mobile chargers and small gadgets</li>
    </ul>
</section>
<section id="dresses" class="section">
    <h2>Dresses Section</h2>
    <p>
        DMart provides a variety of clothing options for all age groups,
        ensuring comfort, quality and affordability.
    </p>

    <ul>
        <li>Men’s casual and formal wear</li>
        <li>Women’s traditional and western wear</li>
        <li>Kids’ clothing and school wear</li>
        <li>Footwear and fashion accessories</li>
        <li>Seasonal and festival collections</li>
    </ul>
</section>
<section id="contact" class="section">
    <h2>Contact Us</h2>
    <p>Email: support@DMart.com</p>
    <p>Phone: +91 98765 43210</p>
</section>

<section id="account" class="section">
    <h2>User Account</h2>
    <p>Login or Register to continue.</p>
</section>


<footer>
    <p>Follow us:
        <a href="#">Instagram</a> |
        <a href="#">Twitter</a> |
        <a href="#">Facebook</a>
    </p>
    <p>© 2026 DMart. All rights reserved.</p>
</footer>

</body>
</html>
```
style.css
```
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: Arial, sans-serif;
}

/* Body */
body {
    background-color: beige;
}

/* Header */
header {
    background-color: black;
    color: green;
    padding: 15px 25px;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

header h1 {
    font-size: 28px;
}

/* Navigation */
nav a {
    color: green;
    margin-left: 18px;
    text-decoration: none;
    font-weight: bold;
    transition: color 0.3s;
}

nav a:hover {
    color: #ff9800;
}

/* Sections */
.section {
    padding: 40px 20px;
    text-align: center;
}

/* Flexbox container */
.flex-container {
    display: flex;
    justify-content: center;
    align-items: stretch;
    gap: 30px;
    flex-wrap: wrap;
}

/* Product Card */
.card {
    background-color: white;
    width: 220px;
    padding: 20px;
    text-align: center;
    box-shadow: 0 0 15px green;
    border-radius: 6px;
    display: flex;
    flex-direction: column;
    align-items: center;
    transition: transform 0.3s;
}

.card:hover {
    transform: scale(1.05);
}

/* Card Images */
.card img {
    width: 100%;
    height: 140px;
    object-fit: contain;
    margin-bottom: 10px;
}

/* Card Headings */
.card h3 {
    color: green;
    margin: 10px 0;
}

/* Card List */
.card ul {
    list-style: none;
    padding: 0;
}

.card ul li {
    font-size: 14px;
    padding: 4px 0;
}

/* Footer */
footer {
    background-color: black;
    color: white;
    text-align: center;
    padding: 15px;
}

footer a {
    color: #ff9800;
    text-decoration: none;
}
.card-link {
    text-decoration: none;
}
html {
    scroll-behavior: smooth;
}
.section ul {
    list-style-type: square;
    max-width: 600px;
    margin: 15px auto;
    text-align: left;
}
body {
    background-color: beige;
    color: green;   /* 🔥 makes ALL text green */
}
h1, h2, h3 {
    color: green;
}
.section, 
.section p, 
.section ul, 
.section li {
    color: green;
}
```
## OUTPUT
![alt text](<Screenshot 2026-02-02 220615.png>)
![alt text](<Screenshot 2026-02-02 222225.png>)
![alt text](<Screenshot 2026-02-02 222240.png>)
## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
