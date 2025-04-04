# portfolio-website
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Your Name - Data Scientist</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <!-- Header -->
    <header>
        <div class="logo">YN</div> <!-- Initials logo -->
        <nav>
            <ul>
                <li><a href="#about">About</a></li>
                <li><a href="#portfolio">Portfolio</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <!-- Homepage -->
    <section id="home">
        <div class="intro">
            <h1>Welcome to My Portfolio</h1>
            <p>I am a Data Scientist with a passion for solving real-world problems through data.</p>
        </div>
    </section>

    <!-- About Me -->
    <section id="about">
        <h2>About Me</h2>
        <p>I specialize in Data Analytics, with a focus on creating actionable insights through data-driven decision-making. My skills include...</p>
    </section>

    <!-- Portfolio -->
    <section id="portfolio">
        <h2>My Work</h2>
        <div class="project-grid">
            <!-- Project example -->
            <div class="project">
                <h3>Project Title</h3>
                <p>Short description of the project.</p>
                <a href="#">View Project</a>
            </div>
            <!-- Repeat for other projects -->
        </div>
    </section>

    <!-- Contact -->
    <section id="contact">
        <h2>Contact Me</h2>
        <form>
            <input type="text" placeholder="Your Name" required>
            <input type="email" placeholder="Your Email" required>
            <textarea placeholder="Your Message" required></textarea>
            <button type="submit">Send Message</button>
        </form>
    </section>

    <!-- Footer -->
    <footer>
        <p>Connect with me on <a href="https://www.linkedin.com">LinkedIn</a></p>
    </footer>

    <script src="script.js"></script>
</body>
</html> 
/* General Reset */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Arial', sans-serif;
    color: #333;
    background-color: #fff;
}

/* Header Styles */
header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1em;
    background-color: maroon;
}

header .logo {
    font-size: 2rem;
    color: white;
    font-weight: bold;
}

nav ul {
    list-style-type: none;
}

nav ul li {
    display: inline;
    margin-left: 20px;
}

nav ul li a {
    color: white;
    text-decoration: none;
}

/* Section Styles */
section {
    padding: 2em 5%;
}

#home {
    background-color: #f4f4f4;
    text-align: center;
}

#about, #portfolio, #contact {
    background-color: #fff;
    margin-bottom: 2em;
}

h2 {
    color: maroon;
}

/* Contact Form Styles */
form input, form textarea {
    width: 100%;
    padding: 0.8em;
    margin-bottom: 1em;
}

button {
    padding: 1em;
    background-color: maroon;
    color: white;
    border: none;
    cursor: pointer;
}

/* Footer Styles */
footer {
    text-align: center;
    background-color: #333;
    color: white;
    padding: 1em;
}
// Simple smooth scroll for navigation links
document.querySelectorAll('a[href^="#"]').forEach(anchor => {
    anchor.addEventListener('click', function (e) {
        e.preventDefault();

        document.querySelector(this.getAttribute('href')).scrollIntoView({
            behavior: 'smooth'
        });
    });
});
