# Ex02 Commercial Website
## Date: 24-08-2025

## AIM:
To create a commercial website using CSS Flexbox.

## ALGORITHM:

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

## PROGRAM:
# Index.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cafe Bliss</title>
    <link rel="stylesheet" href="commercial.css">
</head>
<body>
    <header>
        <nav class="navbar">
            <div class="logo">☕ Cafe Bliss</div>
            <ul class="nav-links">
                <li><a href="#home">Home</a></li>
                <li><a href="#menu">Menu</a></li>
                <li><a href="#specials">Chef's Specials</a></li>
                <li><a href="#order">Order Online</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <section id="home" class="hero">
    <div class="hero-text">
        <h1>Welcome to Cafe Bliss by Hariprasath R</h1>
        <p>Freshly brewed coffee & delightful bakery treats every day!</p>
        <a href="#menu" class="btn explore-btn">🌟 Explore Menu 🌟</a>
    </div>
    <div class="hero-image">
        <img src="images/cafe-hero.png" alt="Cafe Bliss">
    </div>
</section>


    <section id="menu" class="menu">
        <h2>Our Menu</h2>
        <div class="menu-grid">
            <div class="card">
                <img src="images/cappuccino.png" alt="Coffee">
                <h3>Cappuccino</h3>
                <p>Rich espresso with steamed milk foam.</p>
                <span>₹150</span>
            </div>
            <div class="card">
                <img src="images/croissant.png" alt="Croissant">
                <h3>Butter Croissant</h3>
                <p>Flaky and buttery, baked fresh daily.</p>
                <span>₹80</span>
            </div>
            <div class="card">
                <img src="images/cake.png" alt="Cake">
                <h3>Chocolate Cake</h3>
                <p>Decadent and moist, a chocoholic’s dream.</p>
                <span>₹200</span>
            </div>
        </div>
    </section>

    <section id="specials" class="specials">
        <h2>Chef's Specials</h2>
        <div class="specials-grid">
            <div class="card">
                <img src="images/fruit-tart.png" alt="Fruit Tart">
                <h3>Fruit Tart</h3>
                <p>Fresh seasonal fruits with creamy custard.</p>
            </div>
            <div class="card">
                <img src="images/artisan-bread.png" alt="Artisan Bread">
                <h3>Artisan Bread</h3>
                <p>Handmade, crusty, and full of flavor.</p>
            </div>
        </div>
    </section>

    <section id="order" class="order">
        <h2>Order Online</h2>
        <p>Enjoy our delicious treats from the comfort of your home.</p>
        <a href="#" class="btn">Start Ordering</a>
    </section>

    <footer>
        <p>© 2025 Cafe Bliss | Designed with ❤️</p>
        <p>📍 123 Bakery Street, Sweet City, India</p>
        <p>📞 +91 6379005555 | 📧 info@cafebliss.com</p>
        <div class="social-links">
            <a href="#">Facebook</a> | 
            <a href="#">Instagram</a> | 
            <a href="#">Twitter</a>
        </div>
    </footer>
</body>
</html>


```

# commercial.css

```
body {
    margin: 0;
    font-family: Arial, sans-serif;
    color: #333;
}

.navbar {
    background: transparent;
    position: fixed;
    width: 100%;
    padding: 15px 50px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    z-index: 1000;
}

.navbar .logo {
    font-size: 22px;
    font-weight: bold;
    color: white;
}
.nav-links {
    list-style: none;
    display: flex;
    gap: 20px;
}
.nav-links a {
    text-decoration: none;
    color: white;
    transition: 0.3s;
}
.nav-links a:hover {
    color: #ffcc99;
}

.hero {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 80px;
    background: #fdf6f0;
    min-height: 80vh;
}


.hero-text {
    max-width: 50%;
}

.hero-image img {
    width: 400px;   
    border-radius: 20px; 
}



.hero::before {
    content: "";
    position: absolute;
    top: 0; left: 0;
    width: 100%; height: 100%;
    background: rgba(0, 0, 0, 0.45);
    z-index: 1;
}

.hero-text {
    position: relative;
    z-index: 2;
    padding: 20px;
}

.hero-text h1 {
    font-size: 3.5rem;
    font-family: 'Pacifico', cursive;
    background: linear-gradient(90deg, #ffb347, #ffcc33);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    color: transparent;
    text-shadow: 2px 2px 8px rgba(0, 0, 0, 0.4);
    margin-bottom: 10px;
}

.hero-text p {
    font-size: 1.3rem;
    color: #f5f5f5;
    text-shadow: 1px 1px 4px rgba(0,0,0,0.6);
    margin-bottom: 20px;
}

.explore-btn {
    background: linear-gradient(45deg, #ff7e5f, #feb47b);
    color: white;
    font-size: 1.4rem;
    font-weight: bold;
    letter-spacing: 2px;
    padding: 15px 35px;
    border: none;
    border-radius: 50px;
    box-shadow: 0 8px 20px rgba(0,0,0,0.3);
    cursor: pointer;
    transition: all 0.3s ease;
    text-decoration: none;
    display: inline-block;
}

.explore-btn:hover {
    background: linear-gradient(45deg, #feb47b, #ff7e5f);
    transform: scale(1.1);
    box-shadow: 0 10px 25px rgba(0,0,0,0.4);
}

.menu, .specials, .order {
    padding: 50px 20px;
    text-align: center;
}
.menu-grid, .specials-grid {
    display: flex;
    gap: 20px;
    justify-content: center;
    flex-wrap: wrap;
}
.card {
    background: #fff8f0;
    border-radius: 8px;
    overflow: hidden;
    box-shadow: 0 4px 8px rgba(0,0,0,0.2);
    width: 250px;
    padding-bottom: 10px;
    transition: transform 0.3s;
}
.card img {
    width: 100%;
    height: 180px;
    object-fit: cover;
}
.card h3 {
    margin: 10px 0 5px;
}
.card p {
    font-size: 14px;
    padding: 0 10px;
}
.card span {
    font-weight: bold;
    color: #e68a00;
}
.card:hover {
    transform: scale(1.05);
}

.order {
    background: #fff0e6;
}

footer {
    background-color: #5C3A29;
    color: white;
    text-align: center;
    padding: 20px 10px;
    line-height: 1.6;
}

footer p {
    margin: 5px 0;
}

.social-links a {
    color: #f8b878;
    text-decoration: none;
    font-weight: 500;
}

.social-links a:hover {
    color: #ffa366;
}


```


## OUTPUT:

<img width="1919" height="1014" alt="image" src="https://github.com/user-attachments/assets/d7a8f6e3-55c2-49bb-a76e-49cc5fa2951e" />

<img width="1919" height="1014" alt="image" src="https://github.com/user-attachments/assets/515f5cd3-e04a-4013-8ca7-78395b9e43fd" />

<img width="1919" height="1016" alt="image" src="https://github.com/user-attachments/assets/a62f7bce-0990-42d2-95fa-edeb82f6e868" />



## RESULT:
The program for creating commercial website using CSS Flexbox is executed successfully.
