# MDAP-EX_01-Portfolio
## Date: 11-08-2025

## AIM
To create a Portfolio using HTML and CSS.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for introduction, about, projects, and contact details.

### STEP 5
Define global styles for fonts, colors, and layout.

### STEP 6
Style the header, navigation bar, and sections.

### STEP 7
Use Flexbox or CSS Grid for layout design.

### STEP 8
Add hover effects and transitions for interactivity.

### STEP 9
Add Images and Media.

### STEP 10
Use optimized images for a professional look.

### STEP 11
Open the HTML file in a browser to check layout and functionality.

### STEP 12
Fix styling issues and refine content placement.

### STEP 13
Deploy the Portfolio.

### STEP 14
Upload to GitHub Pages for free hosting.

## PROGRAM

index.html

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>Portfolio</title>
    <link rel="stylesheet" href="styles.css" />
</head>
<body>
    <header>
        <h1>My Portfolio</h1>
        <nav>
            <a href="#about">About</a>
            <a href="#projects">Projects</a>
            <a href="#skills">Skills</a>
            <a href="#contact">Contact</a>
        </nav>
    </header>
    <div class="container">
        <section id="about" class="section">
            <h2>About Me</h2>
            <img src="C:\Users\admin\Desktop\portf.jpg" alt="Profile Picture" />
            <p><strong>Zafreen J</strong></p>
            <p>Hi, I am Zafreen Jagir. I am currently pursuing B.E. third year in the department of Computer Science and Engineering at Saveetha Engineering College. My goal is to keep improving, learn new techniques, and build even more complex projects in the future.</p>
        </section>
        <section id="projects" class="section">
            <h2>Projects</h2>
            <ul>
                <li><strong>Project 1:</strong> A responsive website for a local business, built with HTML, CSS, and JavaScript.</li>
                <li><strong>Project 2:</strong> Personal Portfolio Website</li>
                <li><strong>Project 3:</strong> Website for Software Development Company</li>
                <li><strong>Project 4:</strong> Contact Form</li>
            </ul>
        </section>
        <section id="skills" class="section">
            <h2>Skills</h2>
            <div class="skills">
                <div><strong>Java</strong></div>
                <div><strong>C</strong></div>
                <div><strong>Python</strong></div>
                <div><strong>HTML5</strong></div>
                <div><strong>CSS</strong></div>
                <div><strong>JavaScript</strong></div>
                <div><strong>React</strong></div>
                <div><strong>UiPath</strong></div>
            </div>
        </section>
        <section id="contact" class="section">
            <h2>Contact</h2>
            <p>Email: <a href="mailto:zafreen9944@gmail.com">zafreen9944@gmail.com</a></p>
            <p>Github: <a href="https://github.com/ZafreenJagir" target="_blank" rel="noopener noreferrer">https://github.com/ZafreenJagir</a></p>
            <p>LinkedIn: <a href="https://www.linkedin.com/in/ZafreenJagir" target="_blank" rel="noopener noreferrer">www.linkedin.com/in/zafreen-jagir-142280290</a></p>
        </section>
    </div>
    <footer>
        <p>&copy; Zafreen J(212223040252) | <a href="#about">Back to Top</a></p>
    </footer>
</body>
</html>

```

style.css

```
body {
    font-family: 'Arial', sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f4f4f4;
    color: #333;
    line-height: 1.6;
}

header {
    background: linear-gradient(90deg, #333, #555);
    color: #fff;
    padding: 1.5rem 0;
    text-align: center;
    position: sticky;
    top: 0;
    z-index: 1000;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.2);
}

header h1 {
    margin: 0;
    font-size: 2.8rem;
    letter-spacing: 2px;
}

nav {
    margin: 1rem 0;
}

nav a {
    color: #fff;
    text-decoration: none;
    margin: 0 1rem;
    font-weight: bold;
    transition: color 0.3s ease;
}

nav a:hover {
    color: #ffcc00;
}

.container {
    max-width: 1100px;
    margin: 2rem auto;
    background: #fff;
    padding: 2rem;
    border-radius: 10px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
}

.section {
    margin-bottom: 3rem;
}

.section h2 {
    margin-bottom: 1rem;
    color: #333;
    font-size: 2rem;
    border-bottom: 3px solid #333;
    display: inline-block;
    padding-bottom: 0.5rem;
}

.section p,
.section ul {
    font-size: 1.1rem;
    /* Corrected typo: text-align */
    text-align: center;
}

.section ul {
    list-style: none;
    padding: 0;
}

.section ul li {
    background: #f9f9f9;
    margin: 0.5rem 0;
    padding: 0.8rem;
    border-left: 5px solid #333;
    transition: background 0.3s ease;
}

.section ul li:hover {
    background: #f4f4f4;
}

img {
    width: 180px;
    height: 180px;
    border-radius: 50%;
    display: block;
    margin: 1.5rem auto;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
}

.skills {
    display: flex;
    flex-wrap: wrap;
    gap: 1rem;
    margin-top: 1rem;
}

.skills div {
    flex: 1 1 calc(33.333% - 1rem);
    background: #f4f4f4;
    padding: 1rem;
    border-radius: 8px;
    text-align: center;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

.skills div:hover {
    background: #eaeaea;
}

footer {
    text-align: center;
    padding: 1.5rem 0;
    background: #333;
    color: #fff;
    margin-top: 2rem;
}

footer p {
    margin: 0;
    font-size: 0.9rem;
}

footer a {
    color: #ffcc00;
    text-decoration: none;
    font-weight: bold;
}

footer a:hover {
    text-decoration: underline;
}


```


## OUTPUT

<img width="1880" height="1019" alt="image" src="https://github.com/user-attachments/assets/e5029e8e-e0b0-414e-8507-0542a0f774da" />


<img width="1889" height="1032" alt="image" src="https://github.com/user-attachments/assets/5afe8c9b-cf1e-4cd4-954c-58f1a6e65c37" />

<img width="1886" height="1028" alt="image" src="https://github.com/user-attachments/assets/f499a16c-f1a9-4019-a827-7e0415f45adb" />

<img width="1890" height="1027" alt="image" src="https://github.com/user-attachments/assets/96277124-a2e4-413b-9c65-7b49ddcb9f6e" />

## RESULT
The program for creating Portfolio using HTML and CSS is executed successfully.
