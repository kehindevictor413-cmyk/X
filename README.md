<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="A place to read, write, and deepen your understanding.">
    <link rel="stylesheet" href="styles.css">
    <title>Modern Landing Page</title>
</head>
<body>
    <header>
        <nav>
            <div class="logo">YourLogo</div>
            <ul class="nav-menu">
                <li><a href="#">Our Story</a></li>
                <li><a href="#">Membership</a></li>
                <li><a href="#">Write</a></li>
                <li><a href="#">Sign In</a></li>
            </ul>
            <button class="get-started">Get Started</button>
        </nav>
    </header>

    <section class="hero">
        <div class="hero-left">
            <h1>Human stories & ideas</h1>
            <p>A place to read, write, and deepen your understanding</p>
            <button class="cta-button">Start Reading</button>
        </div>
        <div class="hero-right">
            <div class="illustration">
                <!-- Placeholder for illustration -->
                <div class="abstract-shape"></div>
                <div class="line-art"></div>
            </div>
        </div>
    </section>

    <section class="features">
        <div class="feature-card">
            <div class="icon">📝</div>
            <h3>Read Quality Content</h3>
            <p>Explore a variety of topics written by talented authors.</p>
        </div>
        <div class="feature-card">
            <div class="icon">💬</div>
            <h3>Share Your Ideas</h3>
            <p>Write and share your thoughts with a global audience.</p>
        </div>
        <div class="feature-card">
            <div class="icon">🔗</div>
            <h3>Connect With Readers</h3>
            <p>Engage with your audience and build a community.</p>
        </div>
    </section>

    <footer>
        <div class="footer-links">
            <a href="#">Help</a>
            <a href="#">Status</a>
            <a href="#">About</a>
            <a href="#">Careers</a>
            <a href="#">Press</a>
            <a href="#">Blog</a>
            <a href="#">Privacy</a>
            <a href="#">Terms</a>
        </div>
    </footer>
body {
    margin: 0;
    font-family: 'Inter', sans-serif;
    background-color: #F5F3EF;
    color: #000000;
    overflow-x: hidden;
}

header {
    position: fixed;
    width: 100%;
    background: transparent;
    padding: 20px 50px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    transition: background-color 0.3s ease;
}

nav {
    display: flex;
    align-items: center;
}

.logo {
    font-family: 'Playfair Display', serif;
    font-size: 24px;
}

.nav-menu {
    list-style: none;
    display: flex;
    margin: 0;
    padding: 0 20px;
}

.nav-menu li {
    margin-right: 20px;
}

.nav-menu a {
    text-decoration: none;
    color: #000000;
    font-weight: 500;
}

.get-started {
    background: black;
    color: white;
    border: none;
    border-radius: 25px;
    padding: 10px 20px;
    cursor: pointer;
    transition: background 0.3s;
}

.get-started:hover {
    background: #333;
}

.hero {
    display: flex;
    justify-content: space-between;
    padding: 100px 50px;
    margin-top: 80px;
}

.hero-left {
    max-width: 50%;
}

.hero-left h1 {
    font-family: 'Playfair Display', serif;
    font-size: 48px;
}

.hero-left p {
    font-size: 20px;
    margin-top: 10px;
}

.cta-button {
    background: black;
    color: white;
    border: none;
    border-radius: 25px;
    padding: 15px 30px;
    cursor: pointer;
    margin-top: 20px;
    transition: background 0.3s;
}

.cta-button:hover {
    background: #333;
}

.hero-right {
    max-width: 50%;
    position: relative;
}

.illustration {
    position: relative;
}

.abstract-shape {
    width: 200px;
    height: 200px;
    background-color: #25C05A;
    border-radius: 50%;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    animation: float 3s ease-in-out infinite;
}

.line-art {
    width: 150px;
    height: 150px;
    border: 2px solid #000;
    border-radius: 50%;
    position: absolute;
    top: 40%;
    left: 40%;
    transform: translate(-50%, -50%);
    animation: float 2s ease-in-out infinite;
}

@keyframes float {
    0% { transform: translate(-50%, -50%) translateY(0); }
    50% { transform: translate(-50%, -50%) translateY(-10px); }
    100% { transform: translate(-50%, -50%) translateY(0); }
}

.features {
    display: flex;
    justify-content: space-around;
    padding: 50px 50px;
}

.feature-card {
    background: white;
    border-radius: 15px;
    padding: 20px;
    width: 30%;
    text-align: center;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    transition: transform 0.3s;
}

.feature-card:hover {
    transform: translateY(-5px);
}

.footer-links {
    display: flex;
    justify-content: center;
    padding: 20px;
}

.footer-links a {
    margin: 0 15px;
    text-decoration: none;
    color: #6B6B6B;
}
document.addEventListener('DOMContentLoaded', () => {
    // Add smooth scrolling for anchors
    const links = document.querySelectorAll('nav a');
    links.forEach(link => {
        link.addEventListener('click', function(e) {
            e.preventDefault();
            const targetId = this.getAttribute('href');
            const targetSection = document.querySelector(targetId);
            if (targetSection) {
                targetSection.scrollIntoView({ behavior: 'smooth' });
            }
        });
    });
});
    <script src="script.js"></script>
</body>
</html>
