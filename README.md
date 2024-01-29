<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Syed Muhammad Uzair Hussain Shah - Resume</title>
    <style>
        body {
            font-family: 'Verdana', sans-serif;
            line-height: 1.6;
            margin: 20px;
            background: linear-gradient(to right, #3498db, #2c3e50);
            color: #fff;
        }

        header {
            text-align: center;
            margin-bottom: 20px;
        }

        h1 {
            color: #fff;
            margin-bottom: 10px;
            text-decoration: underline;
            font-size: 28px;
        }

        h2 {
            color: #fff;
            border-bottom: 2px solid #fff;
            padding-bottom: 5px;
            margin-top: 20px;
            font-size: 24px;
        }

        p {
            margin-bottom: 10px;
            text-align: justify;
            font-size: 16px;
        }

        ul {
            list-style-type: none;
            padding: 0;
        }

        li {
            margin-bottom: 5px;
            font-size: 16px;
        }

        .contact-info {
            margin-top: 20px;
        }

        nav {
            display: flex;
            justify-content: space-around;
            background-color: #2c3e50;
            padding: 10px;
            margin-bottom: 20px;
            border-radius: 10px;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
        }

        nav a {
            text-decoration: none;
            color: #fff;
            padding: 10px;
            border-radius: 10px;
            background-color: #3498db;
            transition: background-color 0.3s;
            font-size: 18px;
            cursor: pointer;
        }

        nav a:hover {
            background-color: #2980b9;
        }

        section {
            display: none;
            background-color: #2c3e50;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
            color: #fff;
            text-align: justify;
        }

        section.active {
            display: block;
        }

        .personal-info {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .personal-info div {
            flex: 1;
        }

        .qualification-list li,
        .experience-list li,
        .skills-list li {
            padding: 10px 0;
            font-size: 16px;
        }

        .experience-list li:last-child,
        .skills-list li:last-child {
            border-bottom: none;
        }
    </style>
</head>
<body>

    <header>
        <h1>Syed Muhammad Uzair Hussain Shah</h1>
        <p>Content Writer</p>
    </header>

    <nav>
        <a onclick="showTab('personal-info')">Personal Info</a>
        <a onclick="showTab('qualification')">Qualification</a>
        <a onclick="showTab('experience')">Experience</a>
        <a onclick="showTab('skills')">Skills</a>
    </nav>

    <section id="personal-info" class="active">
        <h2>Personal Information</h2>
        <div class="personal-info">
            <div>
                <p><strong>Date of Birth:</strong> 5 May 2001</p>
                <p><strong>Father Name:</strong> Syed Ejaz Hussain Shah</p>
            </div>
            <div>
                <p><strong>Contact Number:</strong> 03472454880</p>
                <p><strong>Email:</strong> uzi4584@gmail.com</p>
            </div>
        </div>
        <p><strong>CNIC Number:</strong> 42201-9883115-9</p>
    </section>

    <section id="qualification">
        <h2>Qualification</h2>
        <ul class="qualification-list">
            <li><strong>Matriculation in Science:</strong> Karachi Board, 2017</li>
            <li><strong>Intermediate in Commerce:</strong> Lahore Board, 2020</li>
        </ul>
    </section>

    <section id="experience">
        <h2>Experience</h2>
        <ul class="experience-list">
            <li><strong>Content Writer</strong> - Vision Tech Internationals Pvt. Ltd., Since January 17, 2022</li>
            <li>Writing descriptions for products and updating those descriptions on the website</li>
            <li>Updating and maintaining products</li>
            <li>Uploading new products to the website</li>
        </ul>
    </section>

    <section id="skills">
        <h2>Skills</h2>
        <ul class="skills-list">
            <li>Creative Content Writing</li>
            <li>Good Communication Skills</li>
        </ul>
    </section>

    <script>
        function showTab(tabId) {
            const sections = document.querySelectorAll('section');
            sections.forEach(section => section.classList.remove('active'));

            const selectedSection = document.getElementById(tabId);
            if (selectedSection) {
                selectedSection.classList.add('active');
            }
        }
    </script>

</body>
</html>
