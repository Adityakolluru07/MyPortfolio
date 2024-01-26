<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
    <title>Aditya Sai Kolluru - Portfolio</title>
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/animate.css">
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css">
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css" integrity="sha384-B4gt1jrGC7Jh4AgTPSdUtOBvfO8sh+WyDLO4NpfDpLq/O/7dz+5z9p5Ff9Kwk8Xr" crossorigin="anonymous">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.1/css/all.min.css" integrity="sha384-mQ93GR66B00ZXjt0YO5KlohRA5SY2XofpXuuYRRf3RB8JcFqF1CJ6uF5dYexlN2" crossorigin="anonymous">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/Chart.js/3.7.0/chart.min.css">
    <script src="https://cdnjs.cloudflare.com/ajax/libs/Chart.js/3.7.0/chart.min.js"></script>

</head>
<style>
    body {
        font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        background-color: #f4f4f4;
        color: #333;
    }

    section {
        padding: 80px 0;
    }

    .jumbotron {
        background-image: url('background-image.jpg');
        background-size: cover;
        color: #ffffff;
        text-align: center;
        padding: 150px 0;
        margin-bottom: 0;
    }

    h1, h2, h3 {
        color: #333;
    }

    .navbar {
        background-color: #1a1a1a;
        padding: 15px 0;
        border-bottom: 2px solid #e44d26;
    }

    .navbar-brand {
        color: #e44d26;
        font-size: 28px;
        position: relative; /* Add this line */
        left: 20px; /* Adjust the left value as needed */
        top: 3px;
        font-style: italic; /* Add this line for italics */
        font-family: 'Playfair Display', serif;
    }

    .navbar-toggler-icon {
        background-color: #e44d26;
    }

    .navbar-nav .nav-item .nav-link {
        color: #ffffff;
        font-size: 18px;
        position: relative; /* Add this line */
        right: 20px; /* Adjust the left value as needed */
        top: 3px;   
    }

    .bg-dark {
        background-color: #1a1a1a;
        color: #ffffff;
    }

    .bg-dark a {
        color: #ffffff;
    }

    .section-title {
        color: #e44d26;
    }

    .animated-text {
        display: inline-block;
    }

    .animated-text span {
        display: inline-block;
        animation: fadeInUp 0.6s ease-out;
    }

    .about-content {
        margin-top: 40px;
    }

    .projects-content {
        margin-top: 60px;
    }

    .project-card {
        margin-bottom: 30px;
        transition: transform 0.3s ease-in-out;
    }

    .project-card:hover {
        transform: scale(1.05);
    }

    .experience-card {
        margin-bottom: 40px;
        transition: transform 0.3s ease-in-out;
    }

    .experience-card:hover {
        transform: scale(1.05);
    }

    .contact-content {
        margin-top: 60px;
    }

    /* Add other styles as needed */

    @keyframes floatBorder {
        0% {
            clip-path: polygon(0 10%, 100% 0, 100% 90%, 0 100%);
        }
        50% {
            clip-path: polygon(0 0, 100% 10%, 100% 90%, 0 100%);
        }
        100% {
            clip-path: polygon(0 10%, 100% 0, 100% 90%, 0 100%);
        }
    }

    .jumbotron {
        background-color: #fff; /* Set background color to white */
        color: #000; /* Set text color to black */
        font-family: 'Arial', sans-serif; /* Change font style as needed */
        position: relative; /* Add this line */
        left: 0px; /* Adjust the left value as needed */
        top: 6px;
        padding: 100px 50px; /* Adjust the top and bottom padding to change the height of the section */
        margin-bottom: 20px; /* Adjust the bottom margin as needed */
    }

    /* Style for the introduction text */
    .intro-text {
        font-size: 18px;
        line-height: 1.6;
        font-weight: normal;
    }
    .display-4 span {
        font-style: italic; /* Add this line for italics */
        font-family: 'Playfair Display', serif;
    }

    .rounded-image {
        width: 250px;
        height: 250px;
        border-radius: 50%; /* Create a circular shape */
        overflow: hidden; /* Hide overflow to maintain the shape */
        margin-right: 20px;
    }

    /* Set a maximum width for the image */
    .rounded-image img {
        width: 100%;
        height: 100%;
        border-radius: 50%;
        object-fit: cover; /* Maintain aspect ratio and cover the container */
        display: block;
    }

    /* Additional CSS for interactive tech stack */
    .tech-stack {
        display: flex;
        align-items: center;
        margin-top: 120px; /* Adjust spacing between intro text and tech stack */
    }

    .tech-stack-title {
        margin-right: 20px; /* Adjust spacing between title and icons */
    }

    .tech-stack-title h3 {
        font-size: 24px; /* Adjust the font size for Tech Stack title */
    }

    .icon-stack {
        display: flex;
        align-items: center;
        gap: 40px; /* Adjust the gap between icons */
    }

    .icon {
        position: relative;
        cursor: pointer;
        transition: transform 0.3s ease-in-out;
    }

    .icon img {
        width: 50px; /* Set the size of your icons */
        height: 50px;
        border-radius: 100%;
    }

    .icon:hover {
        transform: scale(1.2); /* Increase size on hover */
    }

    /* Tooltip for each icon */
    .icon[data-tooltip]:hover::before {
        content: attr(data-tooltip);
        position: absolute;
        top: -30px; /* Adjust the distance of the tooltip from the icon */
        left: 50%;
        transform: translateX(-50%);
        padding: 5px;
        background-color: #333;
        color: #fff;
        border-radius: 5px;
        font-size: 14px;
        opacity: 0.9;
        white-space: nowrap;
    }

    /* Additional CSS to style the emoji */
    .emoji {
        font-style: normal; /* Ensure normal (non-italic) style */
        margin-left: 5px; /* Adjust margin as needed */
    }

    /* Curving the edges of the image */
    .img-fluid.rounded {
        border-radius: 40%; /* You can adjust this percentage for the desired curvature */
    }

    /* Optional: Add some spacing between the image and text */
    .about-content {
        margin-top: 10px;
    }
</style>

<body>

<!-- Navigation Bar -->
<nav class="navbar navbar-expand-lg navbar-dark">
    <a class="navbar-brand" href="#">Aditya Sai Kolluru</a>
    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav"
            aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse justify-content-end" id="navbarNav">
        <ul class="navbar-nav">
            <li class="nav-item">
                <a class="nav-link" href="#about">About</a>
            </li>
            <li class="nav-item">
                <a class="nav-link" href="#projects">Projects</a>
            </li>
            <li class="nav-item">
                <a class="nav-link" href="#experience">Experience</a>
            </li>
            <li class="nav-item">
                <a class="nav-link" href="#contact">Contact</a>
            </li>
        </ul>
    </div>
</nav>



<!-- Introduction Section -->
<div class="jumbotron">
    <div class="container">
        <div class="row">
            <!-- Circular image on the left -->
            <div class="col-md-4">
                <div class="rounded-image">
                    <img src="/Users/adityasaikolluru/Desktop/portfolio/MyPortfolio/src/assets/images/your_photo.jpg" alt="Your Photo">
                </div>
            </div>

            <!-- Text on the right -->
            <div class="col-md-8">
                <h1 class="display-4 animated-text" style="font-family: 'Times New Roman', serif;">
                    <span>Hello!</span>
                    <span class="emoji">&#x1F44B;</span>
                </h1>

                <!-- Introduction -->
                <div class="intro-text">
                    <p>I'm Aditya Kolluru, currently pursuing my Masters in Computer Science at Illinois Institute of Technology. Passionate about developing new distributed applications and predicting knowledge from data to improve future business models.</p>

                    <!-- Tech Stack Introduction with Icons -->
                    <div class="tech-stack">
                        <div class="tech-stack-title">
                            <h3>Tech Stack | </h3>
                        </div>
                        <div class="icon-stack">
                            <div class="icon" data-tooltip="Python Programming">
                                <!-- Icon for Python Programming (You can use an actual icon here) -->
                                <img src="/Users/adityasaikolluru/Desktop/portfolio/MyPortfolio/src/assets/images/Python.png" alt="Python Programming Icon">
                            </div>
                            <div class="icon" data-tooltip="MySQL Database">
                                <!-- Icon for MySQL Database -->
                                <img src="/Users/adityasaikolluru/Desktop/portfolio/MyPortfolio/src/assets/images/MySQL.png" alt="MySQL Database Icon">
                            </div>
                            <div class="icon" data-tooltip="GitHub">
                                <!-- Icon for React -->
                                <img src="/Users/adityasaikolluru/Desktop/portfolio/MyPortfolio/src/assets/images/Git.png" alt="GitHub Icon">
                            </div>
                            <div class="icon" data-tooltip="Data Structure and Algorithms">
                                <!-- Icon for React -->
                                <img src="/Users/adityasaikolluru/Desktop/portfolio/MyPortfolio/src/assets/images/Data Structure and Algorithms.png" alt="Data Structure and Algorithms Icon">
                            </div>
                            <div class="icon" data-tooltip="React">
                                <!-- Icon for React -->
                                <img src="/Users/adityasaikolluru/Desktop/portfolio/MyPortfolio/src/assets/images/React.png" alt="React Icon">
                            </div>
                            
                            <!-- Add more icons and tooltips as needed -->
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</div>


<!-- About Section -->
<section id="about" class="text-center" style="padding: 20px;">
    <div style="max-width: 1150px; margin: 0 auto;">
        <div class="row justify-content-end align-items-center">
            <div class="col-lg-8" style="text-align: center;">
                <h2 style="font-size: 26px; color: #e44d26; margin-bottom: 30px; margin-left: 350px;">About Me</h2>  
                <p style="font-size: 18px; line-height: 1.6; color: rgba(10, 12, 10, 0.954);">
                    Hey, I'm Aditya! 🚀 As a tech explorer and Software Engineer with 3 years of coding adventures, I'm currently navigating the Master's program in Computer Science at Illinois Institute of Technology.
                    I thrive on building innovative distributed applications, weaving technology into the fabric of the future! 💻✨</p>
                
                <!-- Elegant Education Card -->
                <div style="margin-top: 30px;  border-radius: 45px; padding: 10px;">
                    <!-- <h3 style="font-size: 22px; color: #e44d26;">🎓 Education</h3> -->
                    <div style="margin-top: 15px;">
                        <p style="font-size: 16px; line-height: 1.4; color: #333;">📘 <strong>Master's in Computer Science:</strong> Illinois Institute of Technology</p>
                        <p style="font-size: 16px; line-height: 1.4; color: #333;">🎓 <strong>CGPA:</strong> 3.9/4.0</p>
                        <p style="font-size: 16px; line-height: 1.4; color: #333;">🌟 <strong>Preferred Work Location:</strong> Anywhere in the USA fostering creativity and forward-thinking spirit!</p>
                    </div>
                </div>
            </div>
            <div class="col-lg-4" style="margin-top: 20px;">
                <img src="/Users/adityasaikolluru/Desktop/portfolio/MyPortfolio/src/assets/images/CodingImage.png" alt="Your Image Description" style="width: 100%; border-radius: 8px;">
            </div>
        </div>
    </div>
</section>


<!-- Projects Section -->
<style>
    .projects-content {
        margin-top: 30px;
        display: flex;
        flex-wrap: wrap;
        justify-content: space-around;
    }

    .project-link {
        text-decoration: none;
        color: inherit;
    }

    .project-card {
        position: relative;
        overflow: hidden;
        margin-bottom: 20px;
        width: 100%;
        max-width: 300px; /* Adjust the maximum width of the project cards */
    }

    .project-card img {
        width: 100%;
        height: auto;
        transition: transform 0.3s ease-in-out;
        border-radius: 45px; /* Add border-radius for curved edges */
    }

    .project-card:hover img {
        transform: scale(1.1);
    }

    .project-details {
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background: rgba(248, 247, 247, 0.9);
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        opacity: 0;
        transition: opacity 0.3s;
        padding: 20px;
        text-align: center;
        border-radius: 5px; /* Add border-radius for curved edges */
        color: #060606; /* Adjust the text color */
    }

    .project-card:hover .project-details {
        opacity: 1;
    }

    .project-details h3 {
        font-size: 1.5em; /* Adjust the heading size */
        color: #0b0c0c; /* Adjust the heading color */
        margin-bottom: 10px;
    }

    .project-details p {
        font-size: 0.8em; /* Adjust the paragraph size */
        color: #080808; /* Adjust the paragraph color */
        margin: 2px 0;
    }
    .equal-height-card {
        height: 100%; /* You can adjust the height as needed */
    }
    .project-card img {
        width: 100%;
        height: 200px; /* Set a fixed height for all images (adjust the value as needed) */
        object-fit: cover; /* Ensure images maintain their aspect ratio and cover the entire container */
        transition: transform 0.3s ease-in-out;
        border-radius: 45px; /* Add border-radius for curved edges */
    }

</style>

<!-- Projects Section -->
<section id="projects" class="bg-light text-center position-relative">
    <div class="container">
        <h2 class="section-title"> Projects 🚀</h2>
        <!-- Project Cards -->
        <div class="row justify-content-center projects-content">

            <!-- GitHub Insights Dashboard -->
            <div class="col-lg-4 col-md-6 equal-height-card">
                <a href="https://github.com/Adityakolluru07" class="project-link">
                    <div class="project-card">
                        <img src="/Users/adityasaikolluru/Desktop/portfolio/MyPortfolio/src/assets/images/githubInsights.png" alt="GitHub Insights Dashboard">
                        <div class="project-details">
                            <h4>GitHub Insights Dashboard</h4>
                            <p>Created a GitHub Insights Dashboard using Python, Flask, React, Docker, and Google Cloud, leveraging the GitHub API to
                                analyze repository metrics and visualize data with dynamic charts.
                            </p>
                            <p><strong>Skills:</strong> Python, Flask, React, Docker, Google Cloud</p>
                        </div>
                    </div>
                </a>
            </div>

            <!-- Exploring Datasets using Big data Tools -->
            <div class="col-lg-4 col-md-6 equal-height-card">
                <a href="https://github.com/Adityakolluru07" class="project-link">
                    <div class="project-card">
                        <img src="/Users/adityasaikolluru/Desktop/portfolio/MyPortfolio/src/assets/images/Airbnb.png" alt="Big Data Analysis">
                        <div class="project-details">
                            <h4>Big Data Analysis on New York Dataset</h4>
                            <p>EDA using Big Data tools to uncover hidden insights within the Airbnb New York dataset.</p>
                            <p><strong>Tools:</strong> Amazon S3, Apache Spark, Python</p>
                        </div>
                    </div>
                </a>
            </div>

            <!-- Twitter Hate Speech Recognition -->
            <div class="col-lg-4 col-md-6 equal-height-card">
                <a href="https://github.com/Adityakolluru07" class="project-link">
                    <div class="project-card">
                        <img src="/Users/adityasaikolluru/Desktop/portfolio/MyPortfolio/src/assets/images/Twitter.png" alt="Hate Speech Recognition">
                        <div class="project-details">
                            <h4>Twitter Hate Speech Recognition using Machine Learning</h4>
                            <p>Engineered a hate speech classification system employing text normalization, stop word removal, and TF-IDF vectorization.</p>
                            <p><strong>Tools:</strong> Random Forest, TF-IDF</p>
                        </div>
                    </div>
                </a>
            </div>

            <!-- Library Management System -->
            <div class="col-lg-4 col-md-6 equal-height-card">
                <a href="https://github.com/Adityakolluru07" class="project-link">
                    <div class="project-card">
                        <img src="/Users/adityasaikolluru/Desktop/portfolio/MyPortfolio/src/assets/images/Library.png" alt="Library Management System">
                        <div class="project-details">
                            <h3>Library Management System</h3>
                            <p>Crafted a Library Management System with a normalized database, utilizing Postgres SQL and Java Servlet Pages (JSP) on Apache Tomcat.</p>
                            <p><strong>Technologies:</strong> Postgres SQL, Java Servlet Pages (JSP), Apache Tomcat</p>
                        </div>
                    </div>
                </a>
            </div>

        </div>

        <!-- More Projects Coming Soon Text with GitHub link -->
        <div class="position-absolute" style="bottom: 10px; right: 10px; color: #555; font-size: 16px;">
            <a href="https://github.com/Adityakolluru07" style="text-decoration: none; color: inherit;">
                New Projects Coming Soon..🤠 -->
            </a>
        </div>

    </div>
</section>

<!-- Work Experience Section -->
<section id="experience" class="section">
    <div class="container">
        <h2 class="section-title text-center">Work Experience</h2>

        <!-- Accenture - Software Engineer -->
        <div class="experience-timeline">
            <div class="experience-item">
                <div class="experience-meta">
                    <h3>Software Engineer</h3>
                    <p class="location">Accenture, Hyderabad, India | 2019 – 2022</p>
                </div>

                <div class="experience-details">
                    <ul>
                        <li>Spearheaded development of automation solutions for desktop applications in a US-based insurance company.</li>
                        <li>Created an automation suite using visual basic scripting for Oracle EBS and OBIEE, optimizing processes.</li>
                        <li>Demonstrated expertise in CI/CD tools (Git, Jenkins) for seamless integration and continuous delivery.</li>
                        <li>Developed regression scripts, implemented new enhancements, and managed concurrent programs and outbound interfaces.</li>
                        <li>Led strategic initiatives overseeing the complete SDLC, implementing Kanban and Agile methodologies.</li>
                        <li>Utilized agile tools such as Jira and Zephyr (BDD) for efficient project management and collaboration.</li>
                    </ul>
                </div>
            </div>
        </div>

        <!-- Add additional work experiences similarly if needed -->

    </div>
</section>

<!-- Add this script tag to include Chart.js -->
<script src="https://cdn.jsdelivr.net/npm/chart.js"></script>


<section id="skills" class="bg-light text-center py-5">
    <div class="container">
        <h2 class="section-title mb-4">Technical Skills</h2>

        <div class="row justify-content-center">

            <!-- Python Skill -->
            <div class="col-lg-4 mb-4">
                <div class="card skills-card">
                    <div class="card-body">
                        <i class="fab fa-python fa-3x mb-3 text-success"></i>
                        <h5 class="card-title mb-4">Python</h5>
                        <div class="progress">
                            <div class="progress-bar bg-success" role="progressbar" style="width: 90%;" aria-valuenow="90" aria-valuemin="0" aria-valuemax="100">90%</div>
                        </div>
                    </div>
                </div>
            </div>

            <!-- MySQL Skill -->
            <div class="col-lg-4 mb-4">
                <div class="card skills-card">
                    <div class="card-body">
                        <i class="fas fa-database fa-3x mb-3 text-info"></i>
                        <h5 class="card-title mb-4">MySQL</h5>
                        <div class="progress">
                            <div class="progress-bar bg-info" role="progressbar" style="width: 95%;" aria-valuenow="85" aria-valuemin="0" aria-valuemax="100">95%</div>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Java Skill -->
            <div class="col-lg-4 mb-4">
                <div class="card skills-card">
                    <div class="card-body">
                        <i class="fab fa-java fa-3x mb-3 text-warning"></i>
                        <h5 class="card-title mb-4">Java</h5>
                        <div class="progress">
                            <div class="progress-bar bg-warning" role="progressbar" style="width: 60%;" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100">60%</div>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Machine Learning (ML) Skill -->
            <div class="col-lg-4 mb-4">
                <div class="card skills-card">
                    <div class="card-body">
                        <i class="fas fa-robot fa-3x mb-3 text-danger"></i>
                        <h5 class="card-title mb-4">Machine Learning (ML)</h5>
                        <div class="progress">
                            <div class="progress-bar bg-danger" role="progressbar" style="width: 60%;" aria-valuenow="65" aria-valuemin="0" aria-valuemax="100">60%</div>
                        </div>
                    </div>
                </div>
            </div>

            <!-- R Skill -->
            <div class="col-lg-4 mb-4">
                <div class="card skills-card">
                    <div class="card-body">
                        <i class="fab fa-r-project fa-3x mb-3 text-secondary"></i>
                        <h5 class="card-title mb-4">R</h5>
                        <div class="progress">
                            <div class="progress-bar bg-secondary" role="progressbar" style="width: 70%;" aria-valuenow="40" aria-valuemin="0" aria-valuemax="100">70%</div>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Apache Spark Skill -->
            <div class="col-lg-4 mb-4">
                <div class="card skills-card">
                    <div class="card-body">
                        <i class="fab fa-sparkles fa-3x mb-3 text-info"></i>
                        <h5 class="card-title mb-4">Apache Spark</h5>
                        <div class="progress">
                            <div class="progress-bar bg-info" role="progressbar" style="width: 30%;" aria-valuenow="30" aria-valuemin="0" aria-valuemax="100">30%</div>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Apache Hadoop Skill -->
            <div class="col-lg-4 mb-4">
                <div class="card skills-card">
                    <div class="card-body">
                        <i class="fab fa-hubspot fa-3x mb-3 text-warning"></i>
                        <h5 class="card-title mb-4">Apache Hadoop</h5>
                        <div class="progress">
                            <div class="progress-bar bg-warning" role="progressbar" style="width: 25%;" aria-valuenow="25" aria-valuemin="0" aria-valuemax="100">25%</div>
                        </div>
                    </div>
                </div>
            </div>

            <!-- React Skill -->
            <div class="col-lg-4 mb-4">
                <div class="card skills-card">
                    <div class="card-body">
                        <i class="fab fa-react fa-3x mb-3 text-primary"></i>
                        <h5 class="card-title mb-4">React</h5>
                        <div class="progress">
                            <div class="progress-bar bg-primary" role="progressbar" style="width: 20%;" aria-valuenow="20" aria-valuemin="0" aria-valuemax="100">20%</div>
                        </div>
                    </div>
                </div>
            </div>

            <!-- AWS Skill -->
            <div class="col-lg-4 mb-4">
                <div class="card skills-card">
                    <div class="card-body">
                        <i class="fab fa-aws fa-3x mb-3 text-success"></i>
                        <h5 class="card-title mb-4">AWS</h5>
                        <div class="progress">
                            <div class="progress-bar bg-success" role="progressbar" style="width: 30%;" aria-valuenow="30" aria-valuemin="0" aria-valuemax="100">30%</div>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Add more skills as needed -->

        </div>
        <div class="container">
            <p>Few of many soft skills I have:</p>
            <ul class="list-unstyled">
                <p>Self-Motivated, Willingness to Learn, Professionalism, Positive Attitude, Dedication, Hard-Working, Problem-Solving</p>
            </ul>
        </div>
    </div>
</section>




<!-- Contact Section -->

<section id="contact" class=" text-center position-relative">
    <div class="container">
        <h2 class="section-title" style="font-size: 36px; margin-bottom: -30px;">Contact</h2>
        <div class="row justify-content-center contact-content">
            <div class="col-lg-8">
                <p style="font-size: 18px; margin-bottom: 24px;">Feel free to reach out and I will get back to you as soon as possible!! 👇</p>
                <!-- Contact Information -->
                <div class="contact-info">
                    <p style="font-size: 16px; margin-bottom: 20px;">
                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 50 50" style="vertical-align: middle; margin-bottom: 4px;">
                            <path d="M 14 4 C 8.4886661 4 4 8.4886661 4 14 L 4 36 C 4 41.511334 8.4886661 46 14 46 L 36 46 C 41.511334 46 46 41.511334 46 36 L 46 14 C 46 8.4886661 41.511334 4 36 4 L 14 4 z M 13 16 L 37 16 C 37.18 16 37.349766 16.020312 37.509766 16.070312 L 27.679688 25.890625 C 26.199688 27.370625 23.790547 27.370625 22.310547 25.890625 L 12.490234 16.070312 C 12.650234 16.020312 12.82 16 13 16 z M 11.070312 17.490234 L 18.589844 25 L 11.070312 32.509766 C 11.020312 32.349766 11 32.18 11 32 L 11 18 C 11 17.82 11.020312 17.650234 11.070312 17.490234 z M 38.929688 17.490234 C 38.979688 17.650234 39 17.82 39 18 L 39 32 C 39 32.18 38.979687 32.349766 38.929688 32.509766 L 31.400391 25 L 38.929688 17.490234 z M 20 26.410156 L 20.890625 27.310547 C 22.020625 28.440547 23.510234 29 24.990234 29 C 26.480234 29 27.959844 28.440547 29.089844 27.310547 L 29.990234 26.410156 L 37.509766 33.929688 C 37.349766 33.979688 37.18 34 37 34 L 13 34 C 12.82 34 12.650234 33.979687 12.490234 33.929688 L 20 26.410156 z"></path>
                        </svg> 
                        Email: adityakolluru24@gmail.com
                    </p>
                    <p style="font-size: 16px; margin-bottom: 20px;">
                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 50 50" style="vertical-align: middle; margin-bottom: 4px;">
                            <!-- Another SVG code for LinkedIn icon if needed -->
                            <path d="M41,4H9C6.24,4,4,6.24,4,9v32c0,2.76,2.24,5,5,5h32c2.76,0,5-2.24,5-5V9C46,6.24,43.76,4,41,4z M17,20v19h-6V20H17z M11,14.47c0-1.4,1.2-2.47,3-2.47s2.93,1.07,3,2.47c0,1.4-1.12,2.53-3,2.53C12.2,17,11,15.87,11,14.47z M39,39h-6c0,0,0-9.26,0-10 c0-2-1-4-3.5-4.04h-0.08C27,24.96,26,27.02,26,29c0,0.91,0,10,0,10h-6V20h6v2.56c0,0,1.93-2.56,5.81-2.56 c3.97,0,7.19,2.73,7.19,8.26V39z"></path>
                        </svg> 
                        LinkedIn: <a href="https://linkedin.com/in/adityasaikolluru" target="_blank">Aditya Sai Kolluru</a>
                    </p>
                </div>
            </div>
        </div>
    </div>
</section>


<!-- Footer -->
<footer class="bg-dark text-white text-center py-5">
    <div class="container">
        <div class="row">
            <div class="col-md-8 text-left">
                <p>Copyright © 2024 Aditya Kolluru. All rights are reserved</p>
            </div>
            <div class="col-md-4 text-right">
                <a href="https://linkedin.com/in/adityasaikolluru" target="_blank" class="social-link">
                    <!-- Replace with LinkedIn SVG code -->
                    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512" width="40" height="40">
                        <path d="M416 32H31.9C14.3 32 0 46.5 0 64.3v383.4C0 465.5 14.3 480 31.9 480H416c17.6 0 32-14.5 32-32.3V64.3c0-17.8-14.4-32.3-32-32.3zM135.4 416H69V202.2h66.5V416zm-33.2-243c-21.3 0-38.5-17.3-38.5-38.5S80.9 96 102.2 96c21.2 0 38.5 17.3 38.5 38.5 0 21.3-17.2 38.5-38.5 38.5zm282.1 243h-66.4V312c0-24.8-.5-56.7-34.5-56.7-34.6 0-39.9 27-39.9 54.9V416h-66.4V202.2h63.7v29.2h.9c8.9-16.8 30.6-34.5 62.9-34.5 67.2 0 79.7 44.3 79.7 101.9V416z"/>
                    </svg>
                </a>
                <a href="https://github.com/Adityakolluru07" target="_blank" class="social-link">
                    <!-- Replace with GitHub SVG code -->
                    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 496 512" width="40" height="40">
                        <path d="M165.9 397.4c0 2-2.3 3.6-5.2 3.6-3.3 .3-5.6-1.3-5.6-3.6 0-2 2.3-3.6 5.2-3.6 3-.3 5.6 1.3 5.6 3.6zm-31.1-4.5c-.7 2 1.3 4.3 4.3 4.9 2.6 1 5.6 0 6.2-2s-1.3-4.3-4.3-5.2c-2.6-.7-5.5 .3-6.2 2.3zm44.2-1.7c-2.9 .7-4.9 2.6-4.6 4.9 .3 2 2.9 3.3 5.9 2.6 2.9-.7 4.9-2.6 4.6-4.6-.3-1.9-3-3.2-5.9-2.9zM244.8 8C106.1 8 0 113.3 0 252c0 110.9 69.8 205.8 169.5 239.2 12.8 2.3 17.3-5.6 17.3-12.1 0-6.2-.3-40.4-.3-61.4 0 0-70 15-84.7-29.8 0 0-11.4-29.1-27.8-36.6 0 0-22.9-15.7 1.6-15.4 0 0 24.9 2 38.6 25.8 21.9 38.6 58.6 27.5 72.9 20.9 2.3-16 8.8-27.1 16-33.7-55.9-6.2-112.3-14.3-112.3-110.5 0-27.5 7.6-41.3 23.6-58.9-2.6-6.5-11.1-33.3 2.6-67.9 20.9-6.5 69 27 69 27 20-5.6 41.5-8.5 62.8-8.5s42.8 2.9 62.8 8.5c0 0 48.1-33.6 69-27 13.7 34.7 5.2 61.4 2.6 67.9 16 17.7 25.8 31.5 25.8 58.9 0 96.5-58.9 104.2-114.8 110.5 9.2 7.9 17 22.9 17 46.4 0 33.7-.3 75.4-.3 83.6 0 6.5 4.6 14.4 17.3 12.1C428.2 457.8 496 362.9 496 252 496 113.3 383.5 8 244.8 8zM97.2 352.9c-1.3 1-1 3.3 .7 5.2 1.6 1.6 3.9 2.3 5.2 1 1.3-1 1-3.3-.7-5.2-1.6-1.6-3.9-2.3-5.2-1zm-10.8-8.1c-.7 1.3 .3 2.9 2.3 3.9 1.6 1 3.6 .7 4.3-.7 .7-1.3-.3-2.9-2.3-3.9-2-.6-3.6-.3-4.3 .7zm32.4 35.6c-1.6 1.3-1 4.3 1.3 6.2 2.3 2.3 5.2 2.6 6.5 1 1.3-1.3 .7-4.3-1.3-6.2-2.2-2.3-5.2-2.6-6.5-1zm-11.4-14.7c-1.6 1-1.6 3.6 0 5.9 1.6 2.3 4.3 3.3 5.6 2.3 1.6-1.3 1.6-3.9 0-6.2-1.4-2.3-4-3.3-5.6-2z"/>
                    </svg>
                </a>
            </div>
        </div>
    </div>
</footer>


<!-- Bootstrap and JavaScript Scripts -->
<script src="https://code.jquery.com/jquery-3.5.1.slim.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.0.7/dist/umd/popper.min.js"></script>
<script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/wow.js"></script>
<script src="https://code.jquery.com/jquery-3.3.1.slim.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.7/umd/popper.min.js"></script>
<script src="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/js/bootstrap.min.js"></script>

<script>
    new WOW().init();
</script>

</body>
</html>
