AI-Based Traffic Management System for Real-Time Traffic Control

Overview
This project is an AI-powered Smart Traffic Management System that uses real-time vehicle detection to automatically control traffic signals. The system uses a webcam to capture live traffic video and detects vehicles using the YOLOv8 object detection model.
Based on vehicle density, the system automatically changes traffic lights using an Arduino UNO to improve traffic flow and reduce waiting time at intersections.

Features
•	Real-time vehicle detection using YOLOv8
•	Automatic traffic signal control
•	Vehicle counting for multiple road directions
•	Arduino UNO integration for traffic light simulation
•	Low-cost smart traffic solution
•	Improved traffic flow efficiency

Technologies Used
•	Python
•	OpenCV
•	YOLOv8
•	PyTorch
•	Arduino UNO
•	Serial Communication
•	USB Webcam

Working Principle
1. Webcam captures live traffic video.
2. YOLOv8 detects vehicles such as:
•	Cars
•	Bikes
•	Buses
•	Trucks
3. Python counts vehicles on each road.
4. Traffic density is compared.
5. Signal priority is given to the road with higher traffic.
6. Arduino UNO controls traffic LEDs automatically.

System Architecture
Camera → YOLOv8 Detection → Vehicle Counting  
Vehicle Count → Python Logic → Arduino UNO  
Arduino UNO → Traffic Signal LEDs

Algorithm
1. Start the system
2. Capture live video
3. Detect vehicles
4. Count vehicles in Road A and Road B
5. Compare vehicle density
6. Give green signal to higher-density road
7. Update traffic LEDs
8. Repeat continuously

Project Files
•	`vehicle_count_final.py` → Vehicle detection and counting
•	`test_camera.py` → Webcam testing
•	`yolov8n.pt` → YOLO model weights
•	`README.md` → Project documentation

Performance
•	Detection Accuracy: ~85%
•	Processing Speed: 15–20 FPS
•	Improved traffic optimization efficiency in simulated setup

Advantages
•	Real-time traffic management
•	Reduces waiting time
•	Low implementation cost
•	Easy to expand for smart city applications

Limitations
•	Works best in good lighting conditions
•	Depends on webcam quality
•	Current version supports only 2-road intersections

Future Enhancements
•	Emergency vehicle detection
•	Fog and night-mode handling
•	Multi-road intersection support
•	IoT-based cloud monitoring dashboard

Conclusion
This project demonstrates how Artificial Intelligence, Computer Vision, and Embedded Systems can be combined to build a smart traffic control solution for modern urban transportation systems.

System Architecture
<img width="1024" height="558" alt="image" src="https://github.com/user-attachments/assets/c2e69529-d696-432a-b202-4294cf563f60" />
