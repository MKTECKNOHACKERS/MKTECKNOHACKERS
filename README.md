<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Smart Fan System</title>
    <style>
        /* General Styles */
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            margin: 0;
            padding: 0;
            line-height: 1.6;
        }

        header {
            background-color: #333;
            color: white;
            padding: 15px;
            text-align: center;
        }

        nav {
            background-color: #444;
            padding: 10px;
            text-align: center;
        }

        nav a {
            color: white;
            margin: 0 15px;
            text-decoration: none;
            cursor: pointer;
            transition: color 0.3s;
        }

        nav a:hover {
            color: #00bcd4;
        }

        section {
            padding: 20px;
            display: none; /* Hide all sections by default */
        }

        section.active {
            display: block; /* Show the active section */
        }

        ul {
            list-style: none;
            padding: 0;
        }

        ul li {
            margin: 5px 0;
        }
    </style>
</head>
<body>

<header>
    <h1>WELCOME TO MK TECKNO HACKER SITE</h1>
</header>

<nav role="navigation">
    <a onclick="showSection('home')">Home</a>
    <a onclick="showSection('about')">About Us</a>
    <a onclick="showSection('projects')">Our Projects</a>
    <a onclick="showSection('contact')">Contact & Help</a>
</nav>

<section id="home">
    <h2>Welcome to the TECKNO HACKER SITE</h2>
    <p>Welcome to MK Teckno Hacker!
At MK Teckno Hacker, we bring innovation to life by merging technology with practical solutions. Our mission is to create smart, energy-efficient systems that redefine modern living. Explore groundbreaking projects like our Smart Fan System, which leverages IoT and automation to provide seamless temperature control. Join us on a journey to harness technology for a smarter, sustainable future.</p>
</section>

<section id="about">
    <h2>About Us</h2>
    <p>We are MK Teckno Hacker, a team dedicated to creating innovative and energy-efficient solutions for modern living. Our Smart Fan System is a perfect example of our passion for combining technology with practical, real-world applications.</p>
</section>

<section id="projects">
    <h2>Our Projects</h2>
    <p>The Smart Fan System is designed to automate temperature regulation based on sensor readings. It dynamically adjusts the fan motor speed, providing effective cooling or heating solutions based on the temperature. This system also has lighting effects, making it ideal for applications requiring automated thermal management, user customization, and visual indication. The addition of Bluetooth control further enhances the system's usability and remote operability.
:</p>
    <ul>
        <li><strong>Temperature Sensing:</strong> Uses an LMT87LPG temperature sensor to read the ambient temperature and categorize it as either Winter (below 30°C) or Summer (above 30°C).</li>
        <li><strong>Motor Control:</strong> The system controls three motors based on the temperature. Motor 1 adjusts its speed with PWM control, Motor 2 turns on above 33°C, and Motor 3 turns on when the temperature exceeds 50°C.</li>
        <li><strong>LCD Display:</strong> Displays the current temperature and the season (Winter/Summer).</li>
        <li><strong>Bluetooth Communication:</strong> Allows external devices to send temperature data and remotely control the system.</li>
        <li><strong>Energy Efficiency:</strong> The system optimizes motor speed to save energy while ensuring the environment remains at the desired temperature.</li>
    </ul>
</section>

<section id="contact">
    <h2>Contact & Help</h2>
    <p>If you have any questions or need assistance with setting up or using the Smart Fan System, feel free to reach out to us. We're here to help!</p>
    <p><strong>Email:</strong> mktecknohackers@gmail.com</p>
    <p><strong>Phone:</strong> +91 94458 47486</p>
</section>

<script>
    function showSection(sectionId) {
        // Hide all sections
        document.querySelectorAll('section').forEach(section => {
            section.classList.remove('active');
        });

        // Show the clicked section
        document.getElementById(sectionId).classList.add('active');
    }

    // Default: Show the home section when the page loads
    window.addEventListener('DOMContentLoaded', () => showSection('home'));
</script>

</body>
</html>
