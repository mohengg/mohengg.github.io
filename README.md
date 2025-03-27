<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Solar-Powered Surveillance Robot</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #f4f4f4;
            width: 100%;
        }
        header {
            background: #0073e6;
            color: white;
            padding: 15px 0;
            font-size: 24px;
            width: 100%;
        }
        nav {
            background: #005bb5;
            padding: 10px 0;
            width: 100%;
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
            padding: 10px 0;
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
        <a href="#" onclick="showSection('overview')">Project Overview</a>
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
            <p><strong>Method:</strong> Utilize robotics and AI to enhance security measures in various environments.</p>
        </div>
        <div class="info-box" id="features">
            <h2>Key Features</h2>
            <ul>
                <li>Autonomous Navigation: Uses PID control for precise movement and obstacle avoidance.</li>
                <li>Real-Time Monitoring: Captures and transmits video data, detecting nearby persons.</li>
                <li>Solar-Powered: Operates on renewable energy, contributing to sustainability.</li>
            </ul>
        </div>
        <div class="info-box" id="components">
            <h2>Components Used</h2>
            <ul>
                <li><strong>Microcontrollers:</strong> Raspberry Pi Pico (motor control), Raspberry Pi 3 (data processing).</li>
                <li><strong>Sensors:</strong> IR Sensors (path tracking), Ultrasonic Sensor (distance measurement), GPS Module (location tracking), AI Camera (video capture).</li>
            </ul>
        </div>
        <div class="info-box" id="challenges">
            <h2>Technical Challenges</h2>
            <ul>
                <li>Sensor Integration: Ensuring seamless collaboration between components.</li>
                <li>Data Transmission: Efficiently communicating alerts and video feeds.</li>
            </ul>
        </div>
        <div class="info-box" id="benefits">
            <h2>Benefits</h2>
            <ul>
                <li>Enhanced Security: Provides continuous surveillance.</li>
                <li>Energy Efficiency: Utilizes solar power.</li>
                <li>Remote Management: Allows monitoring via Bluetooth.</li>
            </ul>
        </div>
        <div class="info-box" id="future">
            <h2>Future Recommendations</h2>
            <ul>
                <li>Improve AI detection with deep learning techniques like CNN.</li>
                <li>Enhance sensor performance for low-light conditions.</li>
                <li>Integrate SLAM technology for better navigation.</li>
            </ul>
        </div>
    </div>
    <footer>&copy; 2025 Solar-Powered Surveillance Robot</footer>
</body>
</html>
