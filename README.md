<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My GitHub Website</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <nav>
        <div class="logo">MyBrand</div>
        <ul class="nav-links">
            <li><a href="#home">Home</a></li>
            <li><a href="#about">About</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>

    <header id="home">
        <div class="hero">
            <h1>Welcome to My Website</h1>
            <p>Built with passion and hosted on GitHub.</p>
            <button onclick="showAlert()">Click Me</button>
        </div>
    </header>

    <section id="about">
        <h2>About This Project</h2>
        <p>This is a fully responsive starter template for a GitHub Pages site.</p>
    </section>

    <footer>
        <p>&copy; 2026 My GitHub Project</p>
    </footer>
/* General Styles */
body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    margin: 0;
    padding: 0;
    line-height: 1.6;
    color: #333;
}

/* Navigation */
nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    background: #24292e; /* GitHub Dark Gray */
    color: white;
    padding: 1rem 5%;
    position: sticky;
    top: 0;
}

.nav-links {
    list-style: none;
    display: flex;
}

.nav-links li {
    margin-left: 20px;
}

.nav-links a {
    color: white;
    text-decoration: none;
    font-weight: bold;
}

/* Hero Section */
.hero {
    height: 60vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    background: #f4f4f4;
    text-align: center;
    padding: 0 20px;
}

.hero h1 {
    font-size: 3rem;
    margin-bottom: 10px;
}

button {
    padding: 10px 20px;
    font-size: 1rem;
    background: #2ea44f; /* GitHub Green */
    color: white;
    border: none;
    border-radius: 5px;
    cursor: pointer;
}

button:hover {
    background: #2c974b;
}

/* Section Styling */
section {
    padding: 50px 5%;
    text-align: center;
}

footer {
    background: #24292e;
    color: white;
    text-align: center;
    padding: 20px 0;
}
// Simple function to greet the user
function showAlert() {
    alert("Hello! This website is running perfectly on GitHub Pages.");
    console.log("Button was clicked!");
}

// Smooth scrolling for navigation links
document.querySelectorAll('a[href^="#"]').forEach(anchor => {
    anchor.addEventListener('click', function (e) {
        e.preventDefault();
        document.querySelector(this.getAttribute('href')).scrollIntoView({
            behavior: 'smooth'
        });
    });
});

    <script src="script.js"></script>
</body>
</html>
