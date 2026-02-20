<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Elantra Café</title>

<style>
/* --- Reset & Fonts --- */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    background-color: #fdf7f2;
    color: #3b2f2f;
    line-height: 1.6;
}

/* --- Header & Navigation --- */
header {
    background-color: #6f4e37;
    color: #fff;
    padding: 15px 20px;
    position: sticky;
    top: 0;
    z-index: 1000;
}
header nav {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
}
header nav a {
    color: white;
    text-decoration: none;
    margin: 0 20px;
    font-weight: 600;
    padding: 8px 0;
    transition: color 0.3s;
}
header nav a:hover {
    color: #e6c9a8;
}

/* --- Hero Section --- */
.hero {
    background: linear-gradient(rgba(0,0,0,0.4), rgba(0,0,0,0.4)), url('https://images.unsplash.com/photo-1509042239860-f550ce710b93') no-repeat center center/cover;
    color: #fff;
    text-align: center;
    padding: 120px 20px;
}
.hero h1 {
    font-size: 48px;
    margin-bottom: 20px;
}
.hero p {
    font-size: 20px;
    margin-bottom: 30px;
}
.btn {
    background-color: #a67c52;
    color: #fff;
    padding: 12px 25px;
    text-decoration: none;
    border-radius: 6px;
    margin: 5px;
    display: inline-block;
    font-weight: bold;
    transition: background 0.3s;
}
.btn:hover {
    background-color: #8b5c3b;
}

/* --- Sections --- */
.section {
    padding: 60px 20px;
    max-width: 1200px;
    margin: auto;
    text-align: center;
}
.section h2 {
    font-size: 36px;
    margin-bottom: 25px;
    color: #6f4e37;
}

/* --- Menu Grid --- */
.menu-items {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
    gap: 25px;
    justify-items: center;
    margin-top: 30px;
}
.menu-item {
    background: #fffaf4;
    padding: 20px;
    border-radius: 10px;
    box-shadow: 0 6px 15px rgba(0,0,0,0.1);
    transition: transform 0.3s, box-shadow 0.3s;
}
.menu-item:hover {
    transform: translateY(-5px);
    box-shadow: 0 10px 20px rgba(0,0,0,0.15);
}
.menu-item h3 {
    margin-bottom: 10px;
    color: #4b3832;
}
.menu-item p {
    font-weight: bold;
    color: #6f4e37;
}

/* --- FAQ Accordion --- */
.faq {
    max-width: 700px;
    margin: auto;
    text-align: left;
}
details {
    background: #fffaf4;
    margin: 15px 0;
    padding: 15px 20px;
    border-radius: 8px;
    cursor: pointer;
    transition: all 0.3s;
}
details[open] {
    box-shadow: 0 6px 15px rgba(0,0,0,0.1);
}
summary {
    font-weight: bold;
    font-size: 18px;
    outline: none;
}

/* --- Contact Form --- */
form {
    max-width: 600px;
    margin: auto;
    text-align: left;
}
form input, form textarea {
    width: 100%;
    padding: 12px;
    margin: 10px 0;
    border-radius: 6px;
    border: 1px solid #ccc;
    font-size: 16px;
}
form button {
    display: block;
    width: 100%;
    padding: 12px;
    background-color: #a67c52;
    color: #fff;
    border: none;
    font-size: 18px;
    border-radius: 6px;
    cursor: pointer;
    font-weight: bold;
}
form button:hover {
    background-color: #8b5c3b;
}

/* --- Footer --- */
footer {
    background-color: #6f4e37;
    color: #fff;
    padding: 30px 20px;
    text-align: center;
}

/* --- Responsive --- */
@media (max-width: 768px) {
    .hero h1 {
        font-size: 36px;
    }
    .hero p {
        font-size: 18px;
    }
}
</style>
</head>

<body>

<header>
    <nav>
        <a href="#home">Home</a>
        <a href="#about">About</a>
        <a href="#menu">Menu</a>
        <a href="#faq">FAQ</a>
        <a href="#contact">Contact</a>
    </nav>
</header>

<section class="hero" id="home">
    <h1>Welcome to Elantra Café – Where Every Sip Feels Like Home</h1>
    <p>Warm coffee. Cozy atmosphere. Unforgettable moments.</p>
    <a href="#menu" class="btn">View Menu</a>
    <a href="#contact" class="btn">Visit Us</a>
</section>

<section class="section" id="about">
    <h2>About Us</h2>
    <p>Elantra Café is a welcoming space for students, families, and professionals. We serve quality drinks and delicious snacks in a relaxing and friendly environment. Step in and feel at home.</p>
</section>

<section class="section" id="menu">
    <h2>Our Menu</h2>
    <div class="menu-items">
        <div class="menu-item"><h3>Cappuccino</h3><p>₦2,000</p></div>
        <div class="menu-item"><h3>Caramel Latte ⭐</h3><p>₦2,500</p></div>
        <div class="menu-item"><h3>Strawberry Smoothie</h3><p>₦2,500</p></div>
        <div class="menu-item"><h3>Butter Croissant</h3><p>₦1,500</p></div>
        <div class="menu-item"><h3>Chocolate Muffin</h3><p>₦1,800</p></div>
        <div class="menu-item"><h3>Club Sandwich</h3><p>₦3,500</p></div>
    </div>
</section>

<section class="section" id="faq">
    <h2>Frequently Asked Questions</h2>
    <div class="faq">
        <details><summary>Do you offer free WiFi?</summary><p>Yes, fast and free WiFi is available for all customers.</p></details>
        <details><summary>Do you host events?</summary><p>Yes, we host small gatherings, meetings, and birthday parties.</p></details>
        <details><summary>Are there vegetarian options?</summary><p>Yes, our menu includes vegetarian-friendly options.</p></details>
        <details><summary>What are your opening hours?</summary><p>Monday–Friday: 8AM–9PM, Saturday: 9AM–10PM, Sunday: 10AM–8PM</p></details>
        <details><summary>Do you offer delivery?</summary><p>Yes, delivery is available within selected areas.</p></details>
        <details><summary>Can I reserve a table?</summary><p>Yes, you can reserve a table through our contact page or by phone.</p></details>
    </div>
</section>

<section class="section" id="contact">
    <h2>Contact Us</h2>
    <p>Phone: +234 XXX XXX XXXX</p>
    <p>Email: info@elantracafe.com</p>
    <form>
        <input type="text" placeholder="Your Name" required>
        <input type="email" placeholder="Your Email" required>
        <textarea rows="4" placeholder="Your Message" required></textarea>
        <button type="submit">Send Message</button>
    </form>
</section>

<footer>
    <p>© 2026 Elantra Café | All Rights Reserved</p>
</footer>

</body>
</html>
