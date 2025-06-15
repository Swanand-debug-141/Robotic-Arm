Wireless Animatronic Robotic Hand (WOAH)
📌 Project Overview
WOAH (Wireless Operated Animatronic Hand) is a low-cost, wireless robotic hand that mimics human finger gestures using computer vision and servo actuation. The system leverages an Arduino Uno Wi-Fi board, servo motors, and a camera to enable real-time gesture-based control without wired restrictions. This technology finds applications in medical surgeries, hazardous environments, assistive devices, and industrial automation.


🔬 Abstract
This project combines mechatronics, control systems, and computer vision to replicate human hand movements in a robotic hand. The system operates wirelessly and is designed to reduce human involvement in dangerous tasks, assist medical professionals, and aid individuals with disabilities. Gesture input is captured via a camera, processed using Python & OpenCV, and wirelessly transmitted to an Arduino Uno Wi-Fi that drives the servo motors for finger movements.

🛠️ Components Used
Hardware
🎮 Servo Motors (x3–5) – To control finger movement

🔌 Arduino Uno Wi-Fi (with built-in ESP8266) – Main microcontroller and wireless interface

🖐️ Model Hand – Built from plastic coils, metallic strips, and fixed servos

⚡ Jumper Wires and Breadboard – For integration and circuit completion

📷 Web Camera – For gesture recognition

Software
🐍 Python (Computer Vision + Serial Communication)

🧠 OpenCV + cvzone.HandTrackingModule

💻 Arduino IDE (for embedded servo control)

📐 System Architecture
Hand Gesture Capturing – A camera detects the user's finger positions.

Gesture Detection – Python + cvzone module processes the frame in real-time.

Data Transmission – Detected gestures are converted to binary and sent via UART over Wi-Fi.

Arduino Interpretation – Arduino decodes gesture data and activates corresponding servos.

Servo Movement – Robotic fingers mimic human gestures accurately and wirelessly.

💻 Code Overview
Python (Computer Vision)
Uses cvzone.HandTrackingModule to detect hand landmarks.

Converts gesture into a binary list (e.g., [1, 0, 1, 0, 1]).

Sends data to Arduino via serial (UART over USB or Wi-Fi).

Arduino (Embedded Control)
Reads serial binary string.

Maps 0/1 to servo angles (0° or 180°).

Moves fingers based on input pattern.


🎯 Expected Outcome
Wireless control of a robotic hand via finger gestures.

Real-time response with minimal latency.

Reliable performance in tasks like picking, pointing, and gripping.

🧠 Applications
🧪 Hazardous Environments: Bomb disposal, firefighting, nuclear plant operations.

👩‍⚕️ Medical: Remote or minimally invasive surgeries, rehabilitation.

🤖 Industrial Automation: Assembly lines, inspection, machine handling.

🧍 Assistive Tech: Prosthetics for amputees, daily activity aid for disabled individuals.

🌌 Remote Control: Space and deep-sea exploration, disaster recovery.

🧪 Future Improvements
Add movement to the entire hand (wrist, arm).

Improve gesture recognition with ML models.

Miniaturize hardware for wearable or prosthetic use.

Integrate voice commands or brain-computer interfaces.

📷 Working Model
Camera captures hand gesture

Python CV processes image

Data sent to Arduino Uno Wi-Fi

Servo motors adjust robotic hand accordingly

🚀 Getting Started
Prerequisites
Python 3.x

OpenCV (pip install opencv-python)

cvzone (pip install cvzone)

Arduino IDE

USB drivers for Arduino Uno Wi-Fi

🙌 Acknowledgements
Inspired by real-world animatronics and prosthetic research

Special thanks to open-source contributors of cvzone and OpenCV

👨‍💻 Contributors
Swanand Yamgar – Developer & Researcher

![WhatsApp Image 2025-06-15 at 2 18 22 PM](https://github.com/user-attachments/assets/b0660ac6-5347-4b9c-b31c-dd691d810185)
