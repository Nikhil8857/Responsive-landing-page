[8/11, 3:29 PM] Nikhil Borse😎: <!DOCTYPE html>
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
[8/11, 3:30 PM] Nikhil Borse😎: /* Reset some basic styles */
body, h1, h2, h3, p, ul, li, form {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    line-height: 1.6;
}

header {
    background: #333;
    color: #fff;
    padding: 1rem;
}

nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.logo {
    font-size: 1.5rem;
}

.nav-links {
    list-style: none;
    display: flex;
}

.nav-links li {
    margin: 0 1rem;
}

.nav-links a {
    color: #fff;
    text-decoration: none;
}

.hero {
    text-align: center;
    padding: 4rem 1rem;
}

.hero h1 {
    margin-bottom: 0.5rem;
}

.cta-button {
    display: inline-block;
    padding: 0.5rem 1rem;
    background: #007BFF;
    color: #fff;
    text-decoration: none;
    border-radius: 0.25rem;
}

section {
    padding: 2rem;
}

#services {
    background: #f4f4f4;
}

.service-card {
    background: #fff;
    padding: 1rem;
    margin: 1rem 0;
    border-radius: 0.25rem;
    box-shadow: 0 0 10px rgba(0,0,0,0.1);
}

form {
    max-width: 600px;
    margin: auto;
}

form label {
    display: block;
    margin: 0.5rem 0 0.25rem;
}

form input, form textarea {
    width: 100%;
    padding: 0.5rem;
    margin-bottom: 1rem;
}

form button {
    padding: 0.75rem 1.5rem;
    background: #007BFF;
    color: #fff;
    border: none;
    border-radius: 0.25rem;
    cursor: pointer;
}

footer {
    background: #333;
    color: #fff;
    text-align: center;
    padding: 1rem;
}

/* Responsive Styles */
@media (max-width: 768px) {
    .nav-links {
        flex-direction: column;
        align-items: flex-start;
    }

    .nav-links li {
        margin: 0.5rem 0;
    }
}
[8/11, 3:30 PM] Nikhil Borse😎: document.getElementById('contact-form').addEventListener('submit', function(event) {
    event.preventDefault(); // Prevent form from submitting the default way

    const name = document.getElementById('name').value;
    const email = document.getElementById('email').value;
    const message = document.getElementById('message').value;

    if (name && email && message) {
        alert('Thank you for your message, ' + name + '!');
        // Optionally, you can send the form data to a server here
        this.reset(); // Clear the form fields
    } else {
        alert('Please fill out all fields.');
    }
});
