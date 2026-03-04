<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GSMUYANGE | Excellence in Education</title>
    <style>
        /* Base Styling */
        :root {
            --primary-blue: #2c3e50;
            --accent-gold: #f39c12;
            --nursery-red: #e74c3c;
            --primary-green: #27ae60;
            --secondary-blue: #3498db;
            --light-gray: #f4f7f6;
        }

        body {
            font-family: 'Segoe UI', Arial, sans-serif;
            margin: 0;
            padding: 0;
            scroll-behavior: smooth;
            color: #333;
        }

        /* Navigation */
        nav {
            background: var(--primary-blue);
            color: white;
            padding: 15px 5%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            position: sticky;
            top: 0;
            z-index: 1000;
            box-shadow: 0 2px 10px rgba(0,0,0,0.2);
        }

        nav .logo { font-size: 1.6rem; font-weight: bold; letter-spacing: 1px; }
        nav ul { list-style: none; display: flex; margin: 0; }
        nav ul li { margin-left: 25px; }
        nav ul li a { color: white; text-decoration: none; font-weight: 500; transition: 0.3s; }
        nav ul li a:hover { color: var(--accent-gold); }

        /* Hero Section */
        .hero {
            background: linear-gradient(rgba(0,0,0,0.6), rgba(0,0,0,0.6)), 
                        url('https://images.unsplash.com/photo-1546410531-bb4caa1b424d?auto=format&fit=crop&w=1350&q=80');
            background-size: cover;
            background-position: center;
            height: 80vh;
            color: white;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            padding: 0 20px;
        }

        .hero h1 { font-size: 3.5rem; margin-bottom: 10px; }
        .hero p { font-size: 1.2rem; max-width: 600px; }

        /* Sections */
        .container { padding: 60px 10%; text-align: center; }
        h2 { font-size: 2.5rem; margin-bottom: 40px; color: var(--primary-blue); position: relative; }
        h2::after { content: ''; width: 60px; height: 4px; background: var(--accent-gold); position: absolute; bottom: -10px; left: 50%; transform: translateX(-50%); }

        /* Level Cards */
        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            margin-top: 20px;
        }

        .card {
            background: white;
            padding: 30px;
            border-radius: 12px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.1);
            transition: 0.3s;
        }

        .card:hover { transform: translateY(-10px); }
        .card.nursery { border-top: 8px solid var(--nursery-red); }
        .card.primary { border-top: 8px solid var(--primary-green); }
        .card.secondary { border-top: 8px solid var(--secondary-blue); }

        /* Gallery */
        .gallery-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 15px;
        }

        .gallery-grid img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 8px;
            cursor: pointer;
            filter: grayscale(30%);
            transition: 0.3s;
        }

        .gallery-grid img:hover { filter: grayscale(0%); transform: scale(1.03); }

        /* Registration Form */
        .reg-form {
            background: var(--light-gray);
            padding: 40px;
            border-radius: 15px;
            max-width: 800px;
            margin: auto;
            text-align: left;
        }

        .form-group { margin-bottom: 15px; }
        label { display: block; margin-bottom: 5px; font-weight: bold; }
        input, select, textarea {
            width: 100%;
            padding: 12px;
            border: 1px solid #ccc;
            border-radius: 5px;
            box-sizing: border-box;
        }

        .btn {
            background: var(--primary-blue);
            color: white;
            padding: 15px 30px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 1rem;
            width: 100%;
            transition: 0.3s;
        }

        .btn:hover { background: #1a252f; }

        footer {
            background: var(--primary-blue);
            color: white;
            padding: 40px 10%;
            text-align: center;
        }

        .footer-info {
            display: flex;
            justify-content: space-around;
            flex-wrap: wrap;
            margin-bottom: 20px;
        }

        @media (max-width: 768px) {
            nav ul { display: none; } /* Simplified for mobile */
            .hero h1 { font-size: 2.2rem; }
        }
  <style>
    .flag-container {
        display: flex;
        align-items: center;
        gap: 10px;
    }

    .flag {
        width: 40px;
        height: auto;
        border-radius: 2px;
        box-shadow: 0 2px 4px rgba(0,0,0,0.2);
    }

    .header-content {
        display: flex;
        align-items: center;
        gap: 15px;
    }

    /* Animation for the flags */
    .flag:hover {
        transform: scale(1.1);
        transition: 0.3s;
    }
</style>

<nav>
    <div class="header-content">
        <div class="flag-container">
            <img src="https://upload.wikimedia.org/wikipedia/commons/1/17/Flag_of_Rwanda.svg" alt="Rwanda Flag" class="flag">
            <img src="https://cdn-icons-png.flaticon.com/512/5351/5351333.png" alt="GS Muyange Flag" class="flag">
        </div>
        <div class="logo">GSMUYANGE</div>
    </div>
    <ul>
        <li><a href="#home">Home</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#levels">Levels</a></li>
        <li><a href="#gallery">Gallery</a></li>
        <li><a href="#admission">Admission</a></li>
        <li><a href="#contact">Contact</a></li>
    </ul>
</nav>
    <section id="home" class="hero">
        <h1>Educating for Excellence</h1>
        <p>Providing a high-standard learning environment from Nursery to Advanced Secondary levels in Rwanda.</p>
        <a href="#admission" style="margin-top:20px; background:var(--accent-gold); color:white; padding:12px 25px; text-decoration:none; border-radius:5px; font-weight:bold;">Apply Today</a>
    </section>

    <section id="about" class="container">
        <h2>About GS MUYANGE</h2>
        <p>GS MUYANGE is a center of academic brilliance. We are committed to fostering critical thinking, discipline, and creativity in our students. With a team of dedicated teachers and modern facilities, we ensure every child reaches their full potential.</p>
    </section>

    <section id="levels" class="container" style="background-color: #f9f9f9;">
        <h2>Academic Levels</h2>
        <div class="grid">
            <div class="card nursery">
                <h3>Nursery School</h3>
                <p>Early Childhood Education (Years 1-3). We focus on socialization, basic literacy, and numeracy through creative play and modern teaching aids.</p>
            </div>
            <div class="card primary">
                <h3>Primary School</h3>
                <p>Grades P1 to P6. Preparing students for National Examinations with a strong focus on Mathematics, Science, Kinyarwanda, and English.</p>
            </div>
            <div class="card secondary">
                <h3>Secondary School</h3>
                <p><b>O-Level (S1-S3):</b> Broad curriculum foundations.<br><b>A-Level (S4-S6):</b> Specialized combinations in Sciences, Humanities, and Languages.</p>
            </div>
        </div>
    </section>

    <section id="gallery" class="container">
        <h2>School Gallery</h2>
        <div class="gallery-grid">
            <img src="https://images.unsplash.com/photo-1577896851231-70ef18881754?auto=format&fit=crop&w=400&q=80" alt="Classroom">
            <img src="https://images.unsplash.com/photo-1544367567-0f2fcb009e0b?auto=format&fit=crop&w=400&q=80" alt="Students">
            <img src="https://images.unsplash.com/photo-1503676260728-1c00da094a0b?auto=format&fit=crop&w=400&q=80" alt="Library">
            <img src="https://images.unsplash.com/photo-1509062522246-3755977927d7?auto=format&fit=crop&w=400&q=80" alt="Sports">
        </div>
    </section>

    <section id="admission" class="container" style="background: white;">
        <h2>Online Admission</h2>
        <div class="reg-form">
            <form action="#">
                <div class="form-group">
                    <label>Student's Full Name</label>
                    <input type="text" placeholder="Enter name" required>
                </div>
                <div class="form-group">
                    <label>Level Applying For</label>
                    <select required>
                        <option value="">-- Select Level --</option>
                        <option>Nursery</option>
                        <option>Primary</option>
                        <option>Secondary (O-Level)</option>
                        <option>Secondary (A-Level)</option>
                    </select>
                </div>
                <div class="form-group">
                    <label>Parent/Guardian Email</label>
                    <input type="email" placeholder="email@example.com" required>
                </div>
                <div class="form-group">
                    <label>Message/Inquiry</label>
                    <textarea rows="4" placeholder="Tell us more about the student..."></textarea>
                </div>
                <button type="submit" class="btn">Submit Application</button>
            </form>
        </div>
    </section>

    <footer id="contact">
        <div class="footer-info">
            <div>
                <h3>Find Us</h3>
              <p>Muyange,Ruhango,South,Rwanda</p>
            </div>
            <div>
                <h3>Contact Us</h3>
                <p>Phone: +250788836200<br>Email: gsmuyange2@gmail.com</p>
            </div>
            <div>
                <h3>School Hours</h3>
                <p>Mon - Fri: 7:30 AM - 5:00 PM</p>
            </div>
        </div>
        <hr style="opacity: 0.3;">
        <p>&copy; 2026 GS MUYANGE. All Rights Reserved. | Excellence in Rwanda.</p>
    </footer>

</body>
</html>
