<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Solar-Powered Surveillance Robot</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }
        header {
            background: #0073e6;
            color: white;
            padding: 15px;
            font-size: 24px;
        }
        nav {
            background: #005bb5;
            padding: 10px;
        }
        nav a {
            color: white;
            text-decoration: none;
            padding: 10px 15px;
            display: inline-block;
        }
        nav a:hover {
            background: #004494;
            border-radius: 5px;
        }
        .container {
            padding: 20px;
        }
        .info-box {
            background: white;
            padding: 20px;
            margin: 10px auto;
            width: 80%;
            max-width: 600px;
            box-shadow: 0 0 10px rgba(0,0,0,0.1);
            border-radius: 8px;
            text-align: left;
            display: none;
        }
        footer {
            background: #0073e6;
            color: white;
            padding: 10px;
            position: fixed;
            bottom: 0;
            width: 100%;
        }
    </style>
    <script>
        function showSection(sectionId) {
            let sections = document.querySelectorAll(".info-box");
            sections.forEach(section => section.style.display = "none");
            document.getElementById(sectionId).style.display = "block";
        }
    </script>
</head>
<body onload="showSection('overview')">
    <header>Solar-Powered Surveillance Robot</header>
    <nav>
        <a href="#" onclick="showSection('overview')">Overview</a>
        <a href="#" onclick="showSection('features')">Key Features</a>
        <a href="#" onclick="showSection('components')">Components</a>
        <a href="#" onclick="showSection('challenges')">Challenges</a>
        <a href="#" onclick="showSection('benefits')">Benefits</a>
        <a href="#" onclick="showSection('future')">Future Plans</a>
    </nav>
    <div class="container">
        <div class="info-box" id="overview">
            <h2>Project Overview</h2>
            <p><strong>Objective:</strong> Develop an autonomous security robot capable of real-time monitoring and person detection.</p>
            <p><strong>Method:</strong> Utilize robotics and AI technology to enhance security measures in various environments.</p>
        </div>
        <div class="info-box" id="features">
            <h2>Key Features</h2>
            <ul>
                <li>Autonomous Navigation: Uses PID control for precise movement and obstacle avoidance.</li>
                <li>Real-Time Monitoring: Captures and transmits video data, detecting nearby persons.</li>
                <li>Solar-Powered: Operates on renewable energy, contributing to sustainability goals.</li>
            </ul>
        </div>
        <div class="info-box" id="components">
            <h2>Components Used</h2>
            <p><strong>Microcontrollers:</strong></p>
            <ul>
                <li>Raspberry Pi Pico: Handles motor commands.</li>
                <li>Raspberry Pi 3: Manages real-time monitoring and data processing.</li>
            </ul>
            <p><strong>Sensors:</strong></p>
            <ul>
                <li>IR Sensors: For tracking paths and detecting obstacles.</li>
                <li>Ultrasonic Sensor: Measures distance to avoid collisions.</li>
                <li>GPS Module (NEO6MV2): For precise location tracking.</li>
                <li>AI Camera Module: For detecting individuals and capturing video.</li>
            </ul>
        </div>
        <div class="info-box" id="challenges">
            <h2>Technical Challenges</h2>
            <ul>
                <li>Sensor Integration: Ensuring all components work together seamlessly for effective monitoring.</li>
                <li>Data Transmission: Communicating alerts and video feed to users promptly.</li>
            </ul>
        </div>
        <div class="info-box" id="benefits">
            <h2>Benefits</h2>
            <ul>
                <li>Enhanced Security: Reduces human dependency by providing continuous surveillance.</li>
                <li>Energy Efficiency: Utilizes solar power, fostering environmental sustainability.</li>
                <li>Remote Management: Allows users to monitor feeds and control movements via Bluetooth.</li>
            </ul>
        </div>
        <div class="info-box" id="future">
            <h2>Future Recommendations</h2>
            <ul>
                <li>Improve detection algorithms through additional training with deep learning techniques like CNN.</li>
                <li>Incorporate advanced sensors for better performance in low-light and complex environments.</li>
                <li>Explore SLAM technology for improved navigation and adaptability.</li>
            </ul>
        </div>
    </div>
    <footer>&copy; 2025 Solar-Powered Surveillance Robot</footer>
</body>
</html>
