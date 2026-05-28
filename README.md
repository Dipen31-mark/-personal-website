# -personal-website
Your personal website that will include your introduction, education, project description etc. 
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
    <title>Personal Portfolio Website</title>

    <style>
        *{
            margin:0;
            padding:0;
            box-sizing:border-box;
            font-family: Arial, sans-serif;
        }

        html{
            scroll-behavior:smooth;
        }

        body{
            background:#f4f4f4;
            color:#333;
            line-height:1.6;
        }

        /* Navbar */
        header{
            background:#0d6efd;
            padding:15px 50px;
            position:sticky;
            top:0;
            z-index:1000;
        }

        nav{
            display:flex;
            justify-content:space-between;
            align-items:center;
        }

        .logo{
            color:white;
            font-size:28px;
            font-weight:bold;
        }

        .nav-links{
            list-style:none;
            display:flex;
            gap:25px;
        }

        .nav-links a{
            text-decoration:none;
            color:white;
            font-weight:bold;
            transition:0.3s;
        }

        .nav-links a:hover{
            color:#ffd43b;
        }

        /* Hero Section */
        .hero{
            height:90vh;
            background:linear-gradient(rgba(0,0,0,0.6),
            rgba(0,0,0,0.6)),
            url('https://images.unsplash.com/photo-1498050108023-c5249f4df085')
            no-repeat center center/cover;

            display:flex;
            justify-content:center;
            align-items:center;
            text-align:center;
            color:white;
        }

        .hero-content h1{
            font-size:55px;
            margin-bottom:15px;
        }

        .hero-content p{
            font-size:22px;
            margin-bottom:25px;
        }

        .btn{
            display:inline-block;
            padding:12px 30px;
            background:#ffd43b;
            color:black;
            text-decoration:none;
            border-radius:5px;
            font-weight:bold;
            transition:0.3s;
        }

        .btn:hover{
            background:white;
        }

        /* Sections */
        section{
            padding:80px 50px;
        }

        section h2{
            text-align:center;
            margin-bottom:40px;
            color:#0d6efd;
            font-size:38px;
        }

        /* About */
        .about{
            max-width:900px;
            margin:auto;
            text-align:center;
            font-size:18px;
        }

        /* Education */
        .education-container{
            display:flex;
            justify-content:center;
            flex-wrap:wrap;
            gap:25px;
        }

        .edu-card{
            background:white;
            width:300px;
            padding:25px;
            border-radius:10px;
            box-shadow:0 4px 10px rgba(0,0,0,0.1);
            transition:0.3s;
        }

        .edu-card:hover{
            transform:translateY(-8px);
        }

        .edu-card h3{
            color:#0d6efd;
            margin-bottom:10px;
        }

        /* Projects */
        .project-container{
            display:flex;
            justify-content:center;
            flex-wrap:wrap;
            gap:25px;
        }

        .project-card{
            background:white;
            width:320px;
            padding:25px;
            border-radius:10px;
            box-shadow:0 4px 10px rgba(0,0,0,0.1);
            transition:0.3s;
        }

        .project-card:hover{
            transform:scale(1.03);
        }

        .project-card h3{
            color:#0d6efd;
            margin-bottom:15px;
        }

        /* Contact */
        .contact{
            text-align:center;
        }

        .contact p{
            margin:10px 0;
            font-size:18px;
        }

        /* Footer */
        footer{
            background:#222;
            color:white;
            text-align:center;
            padding:25px;
        }

        footer a{
            color:#ffd43b;
            text-decoration:none;
            margin:0 10px;
        }

        footer a:hover{
            text-decoration:underline;
        }

        /* Responsive */
        @media(max-width:768px){

            nav{
                flex-direction:column;
                gap:15px;
            }

            .hero-content h1{
                font-size:38px;
            }

            .hero-content p{
                font-size:18px;
            }

            section{
                padding:60px 20px;
            }
        }
    </style>
</head>
<body>

    <!-- Header/Navbar -->
    <header>
        <nav>
            <div class="logo">MyPortfolio</div>

            <ul class="nav-links">
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#education">Education</a></li>
                <li><a href="#projects">Projects</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <!-- Hero Section -->
    <section class="hero" id="home">
        <div class="hero-content">
            <h1>Hello, I'm Dipen</h1>
            <p>CSE Student | Web Developer | Creative Thinker</p>

            <a href="#projects" class="btn">View Projects</a>
        </div>
    </section>

    <!-- About Section -->
    <section id="about">
        <h2>About Me</h2>

        <div class="about">
            <p>
                I am a passionate Computer Science student who loves
                web development, programming, and creative projects.
                I enjoy learning new technologies and building modern
                and user-friendly websites. My goal is to become a
                skilled software engineer and entrepreneur in the future.
            </p>
        </div>
    </section>

    <!-- Education Section -->
    <section id="education">
        <h2>Education</h2>

        <div class="education-container">

            <div class="edu-card">
                <h3>BSc in Computer Science & Engineering</h3>

                <p><strong>University:</strong> South East University</p>

                <p><strong>Year:</strong> 2024 - Present</p>
            </div>

            <div class="edu-card">
                <h3>Higher Secondary Certificate (HSC)</h3>

                <p><strong>Group:</strong> Science</p>

                <p><strong>Year:</strong> 2023</p>
            </div>

        </div>
    </section>

    <!-- Projects Section -->
    <section id="projects">
        <h2>Projects</h2>

        <div class="project-container">

            <div class="project-card">
                <h3>ZestyGo</h3>

                <p>
                    An online food ordering system project with
                    database management and user-friendly interface.
                </p>
            </div>

            <div class="project-card">
                <h3>ARKO Clothing Brand</h3>

                <p>
                    A creative fashion brand project focused on
                    modern streetwear and online marketing.
                </p>
            </div>

            <div class="project-card">
                <h3>Portfolio Website</h3>

                <p>
                    A responsive personal portfolio website using
                    HTML and CSS to showcase skills and projects.
                </p>
            </div>

        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact">
        <h2>Contact Me</h2>

        <div class="contact">
            <p>Email: dipen@example.com</p>
            <p>Phone: +8801XXXXXXXXX</p>
            <p>Location: Bangladesh</p>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <p>© 2026 Dipen Portfolio Website. All Rights Reserved.</p>

        <br>

        <div>
            <a href="#home">Home</a>
            <a href="#about">About</a>
            <a href="#projects">Projects</a>
        </div>
    </footer>

</body>
</html>
