# MDAP-EX_01-Portfolio
## Date:11.08.2025

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
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Portfolio</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <nav class="navbar">
            <div class="logo">🌟 MyPortfolio</div>
            <ul class="nav-links">
                <li><a href="#" onclick="showSection('home')">Home</a></li>
                <li><a href="#" onclick="showSection('about')">About</a></li>
                <li><a href="#" onclick="showSection('projects')">Projects</a></li>
                <li><a href="#" onclick="showSection('contact')">Contact</a></li>
            </ul>
        </nav>
    </header>
    <section id="home" class="content-section home-section">
        <h1>Hello, I'm <span>Vaishnavi R Nair</span> 👋</h1>
        <p>Creative Web Developer | Designer | Learner</p>
    </section>

    <section id="about" class="content-section about-section" style="display:none;">
        <h2>About Me</h2>
        <img src="vaishuuuu photo.jpg" alt="My Photo" class="profile-pic">
        <p>
           I’m a passionate web developer who thrives on transforming creative ideas into functional, visually engaging digital experiences. 
           With a strong foundation in HTML, CSS, and JavaScript, I enjoy building responsive, user-friendly websites that look great on any device . 
           My design style blends bright colors with clean layouts, ensuring every project is both beautiful and easy to navigate. 
           Beyond coding, I’m constantly learning new technologies, exploring design trends, and experimenting with innovative UI/UX techniques to keep my work fresh and exciting ✨.
        </p>
    </section>

    <section id="projects" class="content-section projects-section" style="display:none;">
        <h2>My Projects</h2>
        <div class="project-container">
            <div class="project-card">
                <h3>🌐 Project One</h3>
                <p>A stunning website built with HTML, CSS, and JavaScript.</p>
            </div>
            <div class="project-card">
                <h3>📱 Project Two</h3>
                <p>A mobile-friendly design that adapts to any screen size.</p>
            </div>
            <div class="project-card">
                <h3>🎨 Project Three</h3>
                <p>A creative and colorful portfolio template.</p>
            </div>
        </div>
    </section>

    <section id="contact" class="content-section contact-section" style="display:none;">
        <h2>Contact Me</h2>
        <p>📧 Email: <a href="mailto:youremail@example.com">vaishnavi.rejish@example.com</a></p>
        <p>📞 Phone: +91 12345 67890</p>
    </section>

    <footer>
        <p>&copy; 2025 Vaishnavi R nair | Made with ❤️</p>
    </footer>
    <script>
        function showSection(sectionId) {
            document.querySelectorAll('.content-section').forEach(sec => {
                sec.style.display = 'none';
            });
            document.getElementById(sectionId).style.display = 'block';
        }
    </script>

</body>
</html>
```
style.css
```
body {
    font-family: 'Segoe UI', sans-serif;
    margin: 0;
    padding: 0;
}
.navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    background: linear-gradient(90deg, #ff5f6d, #ffc371);
    padding: 12px 20px;
}

.logo {
    color: white;
    font-size: 22px;
    font-weight: bold;
}

.nav-links {
    list-style: none;
    display: flex;
    margin: 0;
}

.nav-links li {
    margin: 0 10px;
}

.nav-links a {
    text-decoration: none;
    color: white;
    font-weight: bold;
    padding: 6px 12px;
    border-radius: 6px;
    transition: all 0.3s ease;
}

.nav-links a:hover {
    background: white;
    color: #ff5f6d;
}
.content-section {
    padding: 50px;
    text-align: center;
    min-height: 70vh;
    color: white;
}

.home-section {
    background: linear-gradient(135deg, #667eea, #764ba2);
}

.about-section {
    background: linear-gradient(135deg, #ff758c, #ff7eb3);
}

.projects-section {
    background: linear-gradient(135deg, #43cea2, #185a9d);
}

.contact-section {
    background: linear-gradient(135deg, #f7971e, #ffd200);
}
.project-container {
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
    justify-content: center;
}
.profile-pic {
    width: 150px;
    height: 150px;
    object-fit: cover;
    border-radius: 50%;
    border: 4px solid white;
    box-shadow: 0px 5px 15px rgba(0,0,0,0.3);
}
.project-card {
    background: white;
    color: black;
    padding: 20px;
    border-radius: 10px;
    width: 250px;
    box-shadow: 0 5px 15px rgba(0,0,0,0.2);
    transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.project-card:hover {
    transform: scale(1.05);
    box-shadow: 0 8px 25px rgba(0,0,0,0.3);
}
footer {
    text-align: center;
    background: linear-gradient(90deg, #ff5f6d, #ffc371);
    color: white;
    padding: 10px;
}
a {
    color: white;
    text-decoration: underline;
}
```

## OUTPUT
<img width="1905" height="1050" alt="Screenshot 2025-08-11 120504" src="https://github.com/user-attachments/assets/ccbbfb8b-569a-401b-bd35-96635f635cf4" />
<img width="1907" height="1069" alt="Screenshot 2025-08-11 120514" src="https://github.com/user-attachments/assets/099b0f37-35c8-4bf6-9869-936d26f2fd7b" />
<img width="1917" height="1052" alt="Screenshot 2025-08-11 120527" src="https://github.com/user-attachments/assets/2d7c94ae-44a1-4dc4-8269-0b057d33743d" />
<img width="1917" height="1046" alt="Screenshot 2025-08-11 120553" src="https://github.com/user-attachments/assets/268b3455-126d-4e59-a3e7-5e712687869a" />


## RESULT
The program for creating Portfolio using HTML and CSS is executed successfully.
