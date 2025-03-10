<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pragya Tripathi - Portfolio</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Arial Black', sans-serif;
        }

        body {
            line-height: 1.6;
        }

        /* Navigation */
        nav {
            position: fixed;
            top: 0;
            width: 100%;
            background-color: #333;
            padding: 1rem;
            z-index: 1000;
        }

        nav ul {
            display: flex;
            justify-content: center;
            list-style: none;
        }

        nav ul li {
            margin: 0 1.5rem;
        }

        nav ul li a {
            color: white;
            text-decoration: none;
            font-size: 1.1rem;
        }

        /* Header Section */
        header {
            background: linear-gradient(rgba(0,0,0,0.7), rgba(0,0,0,0.7)), 
                        url('https://cdn.pixabay.com/photo/2016/11/30/20/58/programming-1873854_1280.png');
            height: 100vh;
            color: white;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            padding: 2rem;
        }

        .profile-img {
			width: 150px; /* Adjust as needed */
			height: auto;
			border-radius: 70%;
			box-shadow: 0 0 35px rgba(255, 255, 255, 0.5);
			animation: floatAnimation 3s ease-in-out infinite, glowEffect 1.5s alternate infinite;
		}

		/* Floating effect */
		@keyframes floatAnimation {
		0% {
			transform: translateY(0);
		}
		50% {
			transform: translateY(-10px);
		}
    100% {
			transform: translateY(0);
		}
		}

		/* Glow effect */
		@keyframes glowEffect {
    0% {
        box-shadow: 0 0 10px rgba(255, 255, 255, 0.4);
		}
    100% {
        box-shadow: 0 0 20px rgba(255, 255, 255, 0.8);
		}
		}

        }
		.glow-text {
			font-size: 2em;
			font-weight: bold;
			transition: color 0.3s ease-in-out;
		}

		

		@keyframes colorChange {
			0% { color: red; }
			25% { color: blue; }
			50% { color: green; }
			75% { color: orange; }
			100% { color: purple; }
		}
		
        /* Glow Effect */
        .glow-text {
            font-size: 48px;
            font-weight: bold;
            color: #fff;
            text-align: center;
            animation: glow 1.5s ease-in-out infinite alternate;
        }

        /* Glow Animation */
        @keyframes glow {
            from {
                text-shadow: 0 0 10px #fff, 0 0 20px #fff, 0 0 30px #e60073, 0 0 40px #e60073, 0 0 50px #e60073, 0 0 60px #e60073, 0 0 70px #e60073;
            }
            to {
                text-shadow: 0 0 20px #fff, 0 0 30px #ff4da6, 0 0 40px #ff4da6, 0 0 50px #ff4da6, 0 0 60px #ff4da6, 0 0 70px #ff4da6, 0 0 80px #ff4da6;
            }
        }

        /* Sections */
        section {
            padding: 4rem 2rem;
        }

        .section-title {
            text-align: center;
            margin-bottom: 2rem;
            font-size: 2.5rem;
        }
	/* About section styling */
   /* General styling */
.container {
    position: relative;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    min-height: 100vh;
    overflow: hidden;
}

/* Profile image styling */
.profile-image {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    animation: moveUp 1.5s ease-in-out forwards , fadeOut 1.5s ease-out 2s forwards;
	
}

.profile-image img {
    width: 450px;
    height:450px;
    border-radius: 50%;
    object-fit: cover;
}

/* About content styling */
.about-content {
    opacity: 0;
    transform: translateY(20px);
    animation: fadeIn 1s ease-in-out 1.5s forwards;
    text-align: center;
    max-width: 600px;
    margin-top: 20px;
}

/* Keyframes for image moving up */
@keyframes moveUp {
    0% {
        top: 50%;
    }
    100% {
        top: 20%;
    }
}
@keyframes fadeOut {
            from { opacity: 0; }
            to { opacity: 0; }
        }

/* Keyframes for text fade-in */
@keyframes fadeIn {
    0% {
        opacity: 0;
        transform: translateY(20px);
    }
    100% {
        opacity: 1;
        transform: translateY(0);
    }
}

/* Additional styling for text */
.section-title {
    font-size: 2rem;
    margin-bottom: 1rem;
}

.about-content p {
    font-size: 1rem;
    line-height: 1.6;
    margin-bottom: 1rem;
}

.about-content ul {
    list-style-type: none;
    padding: 0;
}

.about-content ul li {
    margin-bottom: 0.5rem;
}

/* Style each word */
#about p span {
    display: inline-block;
    opacity: 0.5;
    transform: scale(0.8);
    transition: transform 0.3s ease-in-out, opacity 0.3s ease-in-out;
}

/* Apply animation on hover */
#about p:hover span {
    opacity: 1;
    transform: scale(1);
}

/* Adding delay for each word */
#about p span:nth-child(1) { transition-delay: 0s; }
#about p span:nth-child(2) { transition-delay: 0.1s; }
#about p span:nth-child(3) { transition-delay: 0.2s; }
#about p span:nth-child(4) { transition-delay: 0.3s; }
#about p span:nth-child(5) { transition-delay: 0.4s; }
#about p span:nth-child(6) { transition-delay: 0.5s; }
#about p span:nth-child(7) { transition-delay: 0.6s; }
#about p span:nth-child(8) { transition-delay: 0.7s; }

        /* Skills Section */
        
/* Skills Section Styling */
#skills {
    padding: 60px 20px;
    background-color: #f9f9f9;
    text-align: center;
}

.section-title {
    font-size: 2.5rem;
    margin-bottom: 40px;
    color: #333;
}

.skills-container {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 30px;
    max-width: 1000px;
    margin: 0 auto;
}

.skill {
    background: #fff;
    border-radius: 10px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    padding: 20px;
    width: 150px;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
    cursor: pointer;
}

.skill:hover {
    transform: translateY(-10px);
    box-shadow: 0 8px 12px rgba(0, 0, 0, 0.2);
}

.skill i {
    color: #007bff;
    margin-bottom: 15px;
    transition: color 0.3s ease;
}

.skill:hover i {
    color: #0056b3;
}

.skill h3 {
    font-size: 1.2rem;
    color: #333;
    margin: 0;
}

/* Animation for skill items */
@keyframes fadeInUp {
    0% {
        opacity: 0;
        transform: translateY(20px);
    }
    100% {
        opacity: 1;
        transform: translateY(0);
    }
}

.skill {
    opacity: 0;
    animation: fadeInUp 0.5s ease forwards;
}

.skill:nth-child(1) {
    animation-delay: 0.2s;
}

.skill:nth-child(2) {
    animation-delay: 0.4s;
}

.skill:nth-child(3) {
    animation-delay: 0.6s;
}

.skill:nth-child(4) {
    animation-delay: 0.8s;
}

.skill:nth-child(5) {
    animation-delay: 1s;
}
        /* Projects Section */
        
.projects-container {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 20px;
    padding: 20px;
    animation: fadeIn 1s ease-in-out;
}

.project-card {
    display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            margin: 50px auto;
            max-width: 1000px;
            padding: 20px;
        }

        .project-card {
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
            text-align: center;
            transition: transform 0.3s;
        }

        .project-card:hover {
            transform: scale(1.05);
        }

        .project-card img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 10px;
        }
        ul {
            list-style-type: none;
            padding: 0;
        }

        ul li {
            background: #ffe0e6;
            margin: 10px 0;
            padding: 10px;
            border-radius: 5px;
            transition: transform 0.3s;
        }

        ul li:hover {
            transform: scale(1.05);
            background: #ffccd5;
        }

        .fade-in {
            opacity: 0;
            transform: translateY(20px);
            animation: fadeInUp 1.5s ease-in-out forwards;
        }

        @keyframes fadeIn {
            from {
                opacity: 0;
                transform: scale(0.9);
            }
            to {
                opacity: 1;
                transform: scale(1);
            }
        }

        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }


        /* Contact Section */
        .contact-form {
            max-width: 600px;
            margin: 0 auto;
        }

        input, textarea {
            width: 100%;
            padding: 0.5rem;
            margin-bottom: 1rem;
            border: 1px solid #ddd;
        }

        button {
            background: #333;
            color: white;
            padding: 0.7rem 1.5rem;
            border: none;
            cursor: pointer;
        }

        /* Footer */
        /* Footer Styling */
footer {
    background: linear-gradient(135deg, #1e1e1e, #333); /* Gradient Background */
    color: white;
    text-align: center;
    padding: 20px;
    font-size: 16px;
    position: relative;
    animation: fadeInUp 1s ease-in-out;
}

/* Footer Text Glowing Effect */
footer p {
    display: inline-block;
    font-size: 18px;
    font-weight: bold;
    letter-spacing: 1px;
    animation: glowText 2s ease-in-out infinite alternate;
}

/* Hover Effect */
footer:hover {
    transform: scale(1.05); /* Slight bounce effect */
    transition: transform 0.3s ease-in-out;
}

/* Keyframe Animations */
@keyframes fadeInUp {
    from {
        opacity: 0;
        transform: translateY(30px);
    }
    to {
        opacity: 1;
        transform: translateY(0);
    }
}

@keyframes glowText {
    0% {
        text-shadow: 0 0 5px #3e8050, 0 0 10px #35573e, 0 0 15px #35573e;
    }
    100% {
        text-shadow: 0 0 10px #3e8050, 0 0 15px #35573e, 0 0 20px #35573e;
    }
}
/* General Styles */
body {
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  line-height: 1.6;
  margin: 0;
  padding: 0;
  background: linear-gradient(135deg, #f5f7fa, #c3cfe2);
  color: #333;
}

.resume-container {
  max-width: 800px;
  margin: 40px auto;
  padding: 30px;
  background: #fff;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.15);
  border-radius: 12px;
}

/* Profile Section */
.profile-section {
  display: flex;
  align-items: center;
  margin-bottom: 30px;
  padding-bottom: 20px;
  border-bottom: 2px solid #e0e0e0;
}

.profile-image img {
  width: 120px;
  height: 120px;
  border-radius: 50%;
  margin-right: 25px;
  border: 4px solid #4a90e2;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

.profile-info h1 {
  margin: 0;
  font-size: 28px;
  color: #2c3e50;
}

.profile-info p {
  margin: 5px 0 0;
  font-size: 18px;
  color: #7f8c8d;
}

/* Section Styles */
.section {
  margin-bottom: 25px;
}

.section h2 {
  font-size: 22px;
  margin-bottom: 15px;
  color: #2c3e50;
  border-bottom: 2px solid #4a90e2;
  padding-bottom: 8px;
  display: inline-block;
}

.section ul {
  list-style-type: none;
  padding: 0;
}

.section ul li {
  margin-bottom: 12px;
  font-size: 16px;
  padding-left: 20px;
  position: relative;
}

.section ul li::before {
  content: "•";
  color: #4a90e2;
  font-size: 20px;
  position: absolute;
  left: 0;
  top: -2px;
}

/* Additional Personal Info Section */
.additional-info {
  background: #f9f9f9;
  padding: 20px;
  border-radius: 8px;
  margin-top: 20px;
}

.additional-info h2 {
  font-size: 22px;
  margin-bottom: 15px;
  color: #2c3e50;
}

.additional-info ul {
  list-style-type: none;
  padding: 0;
}

.additional-info ul li {
  margin-bottom: 10px;
  font-size: 16px;
  padding-left: 20px;
  position: relative;
}

.additional-info ul li::before {
  content: "•";
  color: #4a90e2;
  font-size: 20px;
  position: absolute;
  left: 0;
  top: -2px;
}

/* Hover Effects */
.profile-image img:hover {
  transform: scale(1.05);
  transition: transform 0.3s ease;
}

.section h2:hover {
  color: #4a90e2;
  transition: color 0.3s ease;
}     
		}
    </style>
</head>
<body>
    <!-- Navigation -->
    <nav>
        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#about">About</a></li>
            <li><a href="#skills">Skills</a></li>
            <li><a href="#projects">Projects</a></li>
			<li><a href="#resume-container">Resume</a></li>
            <li><a href="#contact">Cohntact</a></li>
        </ul>
    </nav>

    <!-- Header Section -->
    <header id="home">
        <img src="C:\Users\aditi\Downloads\Picsart_25-02-08_19-19-28-722.png" class="profile-img" alt="Profile Image">
        <h1 class="glow-text">Pragya Tripathi</h1>
        <p>BCA 2nd Year Student | Aspiring Developer</p>
		<p>I'm a passionate BCA 2nd year student with expertise in programming languages including C, Python, HTML, CSS, and JavaScript. I enjoy creating practical solutions and learning new technologies to enhance my development skills. Passionate creator and meticulous editor with a flair for crafting compelling content. I believe words have the power to inspire, educate, and connect people, and I'm dedicated to harnessing that power to its fullest potential</p>
    </header>

    <!-- About Section -->
    <Section id="about">
        <div class="container">
            <div class="profile-image">
			<img src="C:\Users\aditi\Downloads\Picsart_25-02-08_19-21-23-655.png" alt="Sakshee Chauhan">
			</div>
            <div class="about-content">
                <h2 class="section-title">About Me</h2>
                <p>I am Pragya Tripathi, a passionate and dedicated student currently pursuing my Bachelor’s in Computer Applications (BCA) from Invertis University, Bareilly. My academic journey has allowed me to dive deep into the world of technology, programming, and problem-solving, which has fueled my enthusiasm for coding and software development.</p>
                <p>Since childhood, I have been fascinated by computers, their working mechanisms, and the endless possibilities they offer. This curiosity led me to choose computer applications as my field of study, where I could explore various aspects of software development, database management, web technologies, and problem-solving techniques.</p>
                <h3>My Interest in Coding</h3>
                <p>One of the most exciting aspects of my academic journey has been learning programming languages. I have gained basic knowledge of C, Python, HTML, CSS, and SQL and am constantly working towards improving my skills. The ability to write code and build something from scratch excites me, and I love the process of breaking down complex problems into simple, logical steps.</p>
                <ul>
                    <li><strong>C Programming:</strong> Helped me understand the core concepts of programming, such as loops, functions, arrays, and pointers.</li>
                    <li><strong>Python:</strong> A versatile language that I enjoy using due to its simplicity and powerful libraries.</li>
                    <li><strong>HTML & CSS:</strong> My first step into the world of web development, allowing me to create basic websites.</li>
                    <li><strong>SQL Database:</strong> I have developed an understanding of data storage, retrieval, and management.</li>
                </ul>
                <p>As I continue my studies, I am eager to explore more advanced programming concepts, frameworks, and technologies that will help me become a proficient developer.</p>
            </div>
        </div>
    </section>
        
        <p>.</p>
    </section>

    <!-- Skills Section -->
    <section id="skills">
        <h2 class="section-title">Skills</h2>
        <div class="skills-container">
            <div class="skill">
                <i class="fab fa-c fa-3x"></i>
                <h3>C Programming</h3>
            </div>
            <div class="skill">
                <i class="fab fa-python fa-3x"></i>
                <h3>Python</h3>
            </div>
            <div class="skill">
                <i class="fab fa-html5 fa-3x"></i>
                <h3>HTML5</h3>
            </div>
            <div class="skill">
                <i class="fab fa-css3-alt fa-3x"></i>
                <h3>CSS3</h3>
            </div>
            <div class="skill">
                <i class="fab fa-js fa-3x"></i>
                <h3>JavaScript</h3>
            </div>
        </div>
    </section>

    <!-- Projects Section -->
    <section id="projects">
        <h2 class="section-title">Projects</h2>
        <div class="projects-container">
            <div class="project-card">
                <h3>City Directory (Python)</h3>
				<img src="C:\Users\aditi\Downloads\city-directory-genealogy-salem-e1558710471470.webp" alt="City Directory">
                <p>A console-based application for managing city information and locations using file handling.</p>
                <p class="tech-stack">Tech Stack: Python</p>
            </div>
            <div class="project-card">
                <h3>Portfolio Website</h3>
				<img src="C:\Users\aditi\Downloads\header-2-thompson-chan-1x.webp"alt ="Portfolio Website">
                <p>A responsive personal portfolio website showcasing skills, projects, and contact information.</p>
                <p class="tech-stack">Tech Stack: HTML, CSS, JavaScript</p>
            </div>
            <div class="project-card">
                <h3>Number Guessing Game</h3>
				<img src="C:\Users\aditi\Downloads\rg5pbwrWpN27wrMtQ4VM7I-Yend9ih1bjOrWNieSJdyhJYCVDH3XrDxHqlo-FfEkTSY=w526-h296-rw.webp"alt="Number Guessing Game">
                <p>An interactive game where users guess numbers with score tracking and difficulty levels.</p>
                <p class="tech-stack">Tech Stack: Python</p>
            </div>
        </div>
    </section>
 <!-- REsume-->
 <section id="resume-container">
    <!-- Profile Section -->
    <div class="profile-section">
      <div class="profile-image">
        <img src="profile.jpg" alt="Profile Image">
      </div>
      <div class="profile-info">
        <h1>Your Name</h1>
        <p>BCA Student</p>
      </div>
    </div>

    <!-- Professional Summary -->
    <div class="section">
      <h2>Professional Summary</h2>
      <p>
        Dedicated BCA student with a strong foundation in computer fundamentals and programming languages. 
        I am seeking a role in a company where I can contribute my ideas and be mentored toward a successful career.
      </p>
    </div>

    <!-- Skills -->
    <div class="section">
      <h2>Skills</h2>
      <ul>
        <li>Ms Office (Word, Excel, PowerPoint, etc.)</li>
        <li>Programming Languages (C, Python)</li>
        <li>Communication Skills</li>
        <li>Teamwork</li>
        <li>Time Management</li>
        <li>Flexibility</li>
        <li>Creativity</li>
        <li>Adaptability and Learning</li>
      </ul>
    </div>

    <!-- Education -->
    <div class="section">
      <h2>Education</h2>
      <ul>
        <li>Bachelor of Computer Applications (Pursuing 2nd Year) - Invertis University</li>
        <li>Advanced Diploma in Computer Application (ADCA)</li>
      </ul>
    </div>

    <!-- Certifications -->
    <div class="section">
      <h2>Certifications</h2>
      <ul>
        <li>Certificate of Completion: Artificial Intelligence Fundamentals (Great Learning, September 2024)</li>
        <li>Certificate of Appreciation: Py-WAR (Invertis University, February 2024)</li>
        <li>Certificate of Participation: TechNOVA (2024)</li>
      </ul>
    </div>

    <!-- Additional Personal Info -->
    <div class="section">
      <h2>Additional Personal Info</h2>
      <ul>
        <li>Languages: Hindi, English</li>
        <li>Date of Birth: 2007</li>
        <li>Marital Status: Unmarried</li>
        <li>Nationality: Indian</li>
        <li>Religion: Hindu</li>
        <li>Gender: Female</li>
      </ul>
    </div>
  </Section>
    <!-- Contact Section -->
    <section id="contact">
        <h2 class="section-title">Contact Me</h2>
        <form class="contact-form" id="contactForm">
            <input type="text" placeholder="Name" required>
            <input type="email" placeholder="Email" required>
            <textarea rows="5" placeholder="Message" required></textarea>
            <button type="submit">Send Message</button>
        </form>
    </section>
	
	<section id="personal info">
<div class ="home.sci">
<a href="#"><i class 'bx bxl-instagram'></i></a>
<a href="#"><i class 'bx bxl-linkedin'></i></a>
<a href="#"><i class 'bx bxl-github'></i></a>
</div>
</Section>
<span class="home-imagHover"></span>
</section>

    <!-- Footer -->
    <footer>
        <p>&copy; 2023 Pragya Tripathi. All rights reserved.</p>
    </footer>

    <script>
        // Smooth scrolling for navigation links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });

        // Navigation background change on scroll
        window.addEventListener('scroll', function() {
            const nav = document.querySelector('nav');
            if (window.scrollY > 50) {
                nav.style.backgroundColor = 'rgba(51, 51, 51, 0.9)';
            } else {
                nav.style.backgroundColor = '#333';
            }
        });

        // Form submission
        document.getElementById('contactForm').addEventListener('submit', function(e) {
            e.preventDefault();
            alert('Thank you for your message! I will get back to you soon.');
            this.reset();
        });
		// You can add interactive features here if needed
// For example, a button to toggle dark mode
const toggleDarkMode = () => {
  document.body.classList.toggle("dark-mode");
};

// Example: Add a button to toggle dark mode
const darkModeButton = document.createElement("button");
darkModeButton.innerText = "Toggle Dark Mode";
darkModeButton.addEventListener("click", toggleDarkMode);
document.body.appendChild(darkModeButton);
    </script>
</body>
</html>
