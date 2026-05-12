<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Blue Valley School</title>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <!-- Internal CSS for styling -->
    <style>
        /* Basic Reset */
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }
        body {
            font-family: Arial, Helvetica, sans-serif;
            background: #f8faff;
            color: #092c57;
            line-height: 1.6;
        }

        /* Header and Navigation */
        header {
            background: #1e54a7;
            color: #fff;
            padding: 20px 0;
            box-shadow: 0 2px 6px rgba(30,84,167,0.05);
        }
        .container {
            width: 90%;
            max-width: 960px;
            margin: 0 auto;
        }
        .school-name {
            font-size: 2rem;
            font-weight: bold;
            letter-spacing: 1px;
            margin-bottom: 5px;
        }
        nav {
            margin-top: 8px;
        }
        nav ul {
            list-style: none;
            display: flex;
            gap: 20px;
            flex-wrap: wrap;
        }
        nav ul li a {
            color: #fff;
            text-decoration: none;
            padding: 8px 16px;
            border-radius: 25px;
            transition: background 0.2s;
            font-weight: 500;
        }
        nav ul li a:hover, nav ul li a.active {
            background: #124081;
        }

        /* Section Spacing */
        section {
            padding: 40px 0 20px 0;
            border-bottom: 1px solid #e4eaf4;
        }

        /* Home Section */
        .home-banner {
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 18px;
            margin-top: 10px;
        }
        .home-banner img {
            max-width: 100%;
            width: 350px;
            border-radius: 14px;
            box-shadow: 0 2px 16px rgba(30,84,167,0.09);
        }
        .welcome-message {
            font-size: 1.5rem;
            margin-bottom: 12px;
            text-align: center;
        }
        .show-message-btn {
            background: #1e54a7;
            color: #fff;
            border: none;
            padding: 10px 26px;
            border-radius: 25px;
            font-size: 1rem;
            cursor: pointer;
            margin-top: 10px;
            transition: background 0.2s;
        }
        .show-message-btn:hover {
            background: #1458b3;
        }

        /* About */
        .about-text {
            max-width: 700px;
            margin: 0 auto;
            font-size: 1.07rem;
            background: #e4eaf4;
            padding: 20px;
            border-radius: 10px;
        }

        /* Courses */
        .courses-list {
            display: flex;
            flex-direction: row;
            gap: 22px;
            flex-wrap: wrap;
            justify-content: center;
        }
        .course-card {
            background: #fff;
            border: 1px solid #d1def1;
            border-radius: 12px;
            width: 250px;
            padding: 20px;
            margin-bottom: 18px;
            box-shadow: 0 2px 8px rgba(30,84,167,0.06);
            transition: transform 0.2s;
        }
        .course-card:hover {
            transform: translateY(-6px) scale(1.03);
            box-shadow: 0 4px 16px rgba(30,84,167,0.11);
        }
        .course-title {
            font-size: 1.2rem;
            color: #1e54a7;
            margin-bottom: 7px;
        }
        .course-desc {
            font-size: 0.97rem;
            color: #333;
        }
        
        /* Contact Form */
        .contact-form {
            background: #e4eaf4;
            max-width: 500px;
            margin: 0 auto;
            padding: 22px 24px;
            border-radius: 12px;
        }
        .form-group {
            margin-bottom: 18px;
        }
        .form-group label {
            display: block;
            margin-bottom: 6px;
            font-size: 1rem;
        }
        .form-group input, .form-group textarea {
            width: 100%;
            padding: 9px;
            border-radius: 6px;
            border: 1px solid #b5c9e7;
            font-size: 1rem;
            box-sizing: border-box;
            background: #fff;
            resize: vertical;
        }
        .form-group input:focus, .form-group textarea:focus {
            border: 1.5px solid #1e54a7;
            outline: none;
        }
        .submit-btn {
            background: #1e54a7;
            color: #fff;
            border: none;
            padding: 10px 30px;
            border-radius: 25px;
            font-size: 1rem;
            cursor: pointer;
            transition: background 0.2s;
        }
        .submit-btn:hover {
            background: #1458b3;
        }
        .error-msg {
            color: #ff2255;
            font-size: 0.96rem;
            margin-bottom: 12px;
            display: none;
        }

        /* Footer */
        footer {
            background: #1e54a7;
            color: #fff;
            text-align: center;
            padding: 16px 0;
            font-size: 1rem;
            margin-top: 30px;
        }
        /* Responsive Styles */
        @media (max-width: 700px) {
            .courses-list {
                flex-direction: column;
                align-items: center;
            }
            header, nav ul {
                flex-direction: column;
            }
            .school-name {
                text-align: center;
            }
        }
        @media (max-width: 510px) {
            nav ul {
                flex-direction: column;
                gap: 5px;
                align-items: center;
            }
            .container {
                width: 98%;
                padding: 0 2%;
            }
            .contact-form {
                padding: 15px 6px;
            }
        }
    </style>
</head>
<body>
    <!-- Header with navigation menu -->
    <header>
        <div class="container">
            <div class="school-name">Blue Valley School</div>
            <nav>
                <ul>
                    <li><a href="#home" class="active">Home</a></li>
                    <li><a href="#about">About</a></li>
                    <li><a href="#courses">Courses</a></li>
                    <li><a href="#contact">Contact</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- Home Section -->
    <section id="home">
        <div class="container home-banner">
            <div class="welcome-message">
                Welcome to Blue Valley School!  
                <br>Building bright futures since 1995.
            </div>
            <!-- Banner image (public domain/illustrative) -->
            <img src="https://images.unsplash.com/photo-1503676382389-4809596d5290?auto=format&fit=crop&w=600&q=80" 
                 alt="School Banner">
            <!-- Interactive button (JS will show a message) -->
            <button class="show-message-btn" onclick="showSchoolWelcome()">Show School Welcome</button>
            <div id="school-message" style="font-weight:500; color:#2171d3; margin-top: 12px; display:none;"></div>
        </div>
    </section>
    
    <!-- About Section -->
    <section id="about">
        <div class="container">
            <h2>About Us</h2>
            <div class="about-text">
                Blue Valley School is dedicated to nurturing lifelong learners and responsible citizens.<br><br>
                <b>Our Vision:</b> To inspire every student to achieve excellence in academics and character. <br><br>
                <b>Our Community:</b> We provide a safe, supportive environment where educators and students flourish side by side.
            </div>
        </div>
    </section>

    <!-- Courses Section -->
    <section id="courses">
        <div class="container">
            <h2>Our Courses</h2>
            <div class="courses-list">
                <!-- Course 1 -->
                <div class="course-card">
                    <div class="course-title">Mathematics Excellence</div>
                    <div class="course-desc">Engage with hands-on lessons and problem-solving to build confidence and love for math.</div>
                </div>
                <!-- Course 2 -->
                <div class="course-card">
                    <div class="course-title">Creative Sciences</div>
                    <div class="course-desc">Explore the wonders of biology, chemistry, and physics through experiments and projects.</div>
                </div>
                <!-- Course 3 -->
                <div class="course-card">
                    <div class="course-title">Arts & Communication</div>
                    <div class="course-desc">Develop creative expression with visual arts, music, and public speaking workshops.</div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact">
        <div class="container">
            <h2>Contact Us</h2>
            <form class="contact-form" id="contactForm" autocomplete="off">
                <div class="error-msg" id="formError"></div>
                <div class="form-group">
                    <label for="name">Name*</label>
                    <input type="text" id="name" name="name" placeholder="Your Name">
                </div>
                <div class="form-group">
                    <label for="email">Email*</label>
                    <input type="email" id="email" name="email" placeholder="your@email.com">
                </div>
                <div class="form-group">
                    <label for="message">Message*</label>
                    <textarea id="message" name="message" rows="4" placeholder="Type your message here"></textarea>
                </div>
                <button type="submit" class="submit-btn">Send Message</button>
            </form>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        &copy; 2026 Blue Valley School. All rights reserved.
    </footer>

    <!-- Internal JavaScript for interaction and form validation -->
    <script>
        // Navigation: Add 'active' class to clicked link
        const navLinks = document.querySelectorAll("nav ul li a");
        navLinks.forEach(link => {
            link.addEventListener("click", function() {
                navLinks.forEach(l => l.classList.remove("active"));
                this.classList.add("active");
            });
        });

        // JavaScript: Show a welcome message when button is clicked
        function showSchoolWelcome() {
            document.getElementById('school-message').style.display = "block";
            document.getElementById('school-message').innerText = "Welcome to our school!";
        }

        // Contact Form Validation
        document.getElementById('contactForm').addEventListener('submit', function(e){
            e.preventDefault(); // Prevent actual form submit
            
            // Get input values and form error element
            var name = document.getElementById('name').value.trim();
            var email = document.getElementById('email').value.trim();
            var message = document.getElementById('message').value.trim();
            var errorDiv = document.getElementById('formError');
            
            // Validate fields
            let errorMsg = '';
            if (name === '' || email === '' || message === '') {
                errorMsg = "Please fill out all required fields.";
            } else if (!validateEmail(email)) {
                errorMsg = "Please enter a valid email address.";
            }
            
            if (errorMsg) {
                errorDiv.style.display = 'block';
                errorDiv.innerText = errorMsg;
                return;
            }
            
            // If valid, show success alert and reset form
            errorDiv.style.display = 'none';
            alert("Thank you for contacting us, " + name + "! We have received your message.");
            this.reset();
        });

        // Simple email validation function
        function validateEmail(email) {
            // Basic regex for email validation
            var re = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
            return re.test(email);
        }
    </script>
</body>
</html>
