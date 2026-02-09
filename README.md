Agrobot: Touch-driven Autonomous Farming 🌾🤖
Agrobot is an intuitive Human-Robot Interaction (HRI) platform that allows farmers to navigate agricultural robots using Augmented Reality (AR). By shifting from complex GPS coordinates to a simple "touch-to-draw" interface, Agrobot makes precision farming accessible to users with zero technical background.

🌟 The Concept
Traditional autonomous farming requires expensive RTK-GPS and complex mapping software. Agrobot simplifies this:
Point: Open the web app and point the camera at the field.
Touch: Draw a path directly on the screen over the live video feed of the ground.
Go: The robot autonomously follows the visually mapped path to perform tasks like weeding or spraying.

🛠️ Technical Stack (CSE Architecture)
AR Interface: AR.js & A-Frame (Web-based Augmented Reality)
Cloud Sync: Firebase Realtime Database (NoSQL)
Microcontroller: NodeMCU (ESP8266) (IoT Gateway)
Firmware: Written in C++ via Arduino IDE
Hardware: L298N Motor Driver, High-torque DC Motors, 4WD Chassis.

📂 Project Workflow
Surface Tracking: The browser uses WebAR to detect the ground plane and create a 3D coordinate system.
Path Mapping: JavaScript captures touch events, converting screen pixels into X and Z world coordinates.
IoT Bridge: Coordinates are pushed to Firebase as a JSON array.
Execution: The NodeMCU fetches the array via Wi-Fi and converts the distance data into motor pulse-width modulation (PWM) signals.

🚀 Key Innovation (Novelty)
Zero-Code Interface: No programming or GPS knowledge required.
Hardware Agnostic: Works on any smartphone browser (Chrome/Safari) without app installation.
Dynamic Obstacle Avoidance: Farmers can visually see obstacles and draw paths around them in real-time.

🔧 Installation
Clone Repository: git clone https://github.com
Hosting: Upload index.html to GitHub Pages for a live AR link.
Hardware: Flash the code in /src/hardware.ino to your NodeMCU.

📄 License
This project is licensed under the MIT License.
Project Lead: [KAVIYA S]
Degree: B.E. Computer Science and Engineering
Timeline: Feb 2026 - Apr 2026
