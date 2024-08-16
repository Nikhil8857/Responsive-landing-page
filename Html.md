<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Responsive Landing Page</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <nav>
            <div class="logo">MySite</div>
            <ul class="nav-links">
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#services">Services</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
        <div class="hero">
            <h1>Welcome to MySite</h1>
            <p>Your journey to excellence starts here.</p>
            <a href="#contact" class="cta-button">Get Started</a>
        </div>
    </header>

    <section id="about">
        <h2>About Us</h2>
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam ac urna vel erat cursus auctor.</p>
    </section>

    <section id="services">
        <h2>Our Services</h2>
        <div class="service-card">
            <h3>Service 1</h3>
            <p>Description of service 1.</p>
        </div>
        <div class="service-card">
            <h3>Service 2</h3>
            <p>Description of service 2.</p>
        </div>
        <div class="service-card">
            <h3>Service 3</h3>
            <p>Description of service 3.</p>
        </div>
    </section>

    <section id="contact">
        <h2>Contact Us</h2>
        <form id="contact-form">
            <label for="name">Name:</label>
            <input type="text" id="name" name="name" required>
            
            <label for="email">Email:</label>
            <input type="email" id="email" name="email" required>
            
            <label for="message">Message:</label>
            <textarea id="message" name="message" required></textarea>
            
            <button type="submit">Send</button>
        </form>
    </section>

    <footer>
        <p>&copy; 2024 MySite. All rights reserved.</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>
