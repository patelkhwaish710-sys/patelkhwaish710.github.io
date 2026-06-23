<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>patel khwaish | Web Developer Portfolio</title>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:'Poppins',sans-serif;
}

html{
    scroll-behavior:smooth;
}

body{
    background:#0a0f1f;
    color:white;
}

/* Navbar */
nav{
    position:fixed;
    width:100%;
    top:0;
    background:rgba(0,0,0,0.85);
    backdrop-filter:blur(10px);
    padding:15px 10%;
    display:flex;
    justify-content:space-between;
    align-items:center;
    z-index:1000;
}

.logo{
    font-size:24px;
    font-weight:bold;
    color:#00f7ff;
}

nav ul{
    display:flex;
    list-style:none;
    gap:20px;
}

nav a{
    color:white;
    text-decoration:none;
    transition:.3s;
}

nav a:hover{
    color:#00f7ff;
}

/* Hero */
.hero{
    min-height:100vh;
    display:flex;
    align-items:center;
    justify-content:center;
    text-align:center;
    padding:50px;
}

.hero-content h1{
    font-size:60px;
}

.hero-content h1 span{
    color:#00f7ff;
}

.hero-content p{
    margin:20px 0;
    font-size:18px;
    color:#cfcfcf;
}

.btn{
    display:inline-block;
    padding:12px 30px;
    background:#00f7ff;
    color:black;
    border-radius:30px;
    text-decoration:none;
    font-weight:bold;
    transition:.3s;
}

.btn:hover{
    transform:translateY(-5px);
}

/* Sections */
section{
    padding:90px 10%;
}

.section-title{
    text-align:center;
    font-size:35px;
    margin-bottom:40px;
    color:#00f7ff;
}

/* About */
.about{
    text-align:center;
    line-height:1.8;
}

/* Skills */
.skills-container{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(200px,1fr));
    gap:20px;
}

.skill{
    background:#141d35;
    padding:25px;
    border-radius:15px;
    text-align:center;
    transition:.3s;
}

.skill:hover{
    transform:translateY(-10px);
}

/* Projects */
.projects{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(280px,1fr));
    gap:25px;
}

.project-card{
    background:#141d35;
    padding:25px;
    border-radius:15px;
    transition:.3s;
}

.project-card:hover{
    transform:scale(1.05);
}

.project-card h3{
    color:#00f7ff;
    margin-bottom:10px;
}

/* Contact */
.contact{
    text-align:center;
}

.contact p{
    margin:10px;
}

footer{
    text-align:center;
    padding:20px;
    background:#060b17;
    color:#aaa;
}

/* Responsive */
@media(max-width:768px){
    .hero-content h1{
        font-size:40px;
    }

    nav{
        flex-direction:column;
        gap:10px;
    }
}
</style>
</head>
<body>

<nav>
    <div class="logo">khwaish.</div>
    <ul>
        <li><a href="#about">About</a></li>
        <li><a href="#skills">Skills</a></li>
        <li><a href="#projects">Projects</a></li>
        <li><a href="#contact">Contact</a></li>
    </ul>
</nav>

<!-- Hero -->
<section class="hero">
    <div class="hero-content">
        <h1>Hello, I'm <span>patel khwaish </span></h1>
        <p id="typing"></p>
        <a href="#projects" class="btn">View My Work</a>
    </div>
</section>

<!-- About -->
<section id="about">
    <h2 class="section-title">About Me</h2>
    <div class="about">
        <p>
            I am an IT Diploma Student passionate about Web Development,
            Cyber Security and Modern Technologies.
            I enjoy building responsive websites and learning new tools.
        </p>
    </div>
</section>

<!-- Skills -->
<section id="skills">
    <h2 class="section-title">Skills</h2>

    <div class="skills-container">
        <div class="skill">HTML5</div>
        <div class="skill">CSS3</div>
        <div class="skill">JavaScript</div>
        <div class="skill">Java</div>
        <div class="skill">SQL</div>
        <div class="skill">JDBC</div>
        <div class="skill">JSP</div>
        <div class="skill">Git & GitHub</div>
    </div>
</section>

<!-- Projects -->
<section id="projects">
    <h2 class="section-title">Projects</h2>

    <div class="projects">

        <div class="project-card">
            <h3>Portfolio Website</h3>
            <p>
                Personal portfolio built using HTML, CSS and JavaScript
                showcasing skills and projects.
            </p>
        </div>

        <div class="project-card">
            <h3>Login System</h3>
            <p>
                Responsive Login & Signup Form with modern UI design.
            </p>
        </div>

        <div class="project-card">
            <h3>Student Database</h3>
            <p>
                Java, JDBC and SQL based student management application.
            </p>
        </div>

    </div>
</section>

<!-- Contact -->
<section id="contact">
    <h2 class="section-title">Contact</h2>

    <div class="contact">
        <p>📧 aasthachauhan1308@gmail.com</p>
        <p>📍 Gujarat, India</p>
        <p>💻 Web Developer & Cyber Security Learner</p>
    </div>
</section>

<footer>
    © 2026 patel khwaish | All Rights Reserved
</footer>

<script>
const text =
"Frontend Developer • Java Programmer • Cyber Security Learner";

let i = 0;

function typeWriter(){
    if(i < text.length){
        document.getElementById("typing").innerHTML += text.charAt(i);
        i++;
        setTimeout(typeWriter,70);
    }
}
typeWriter();
</script>

</body>
</html>
