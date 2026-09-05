# Smart Gate: Computer Vision & IoT-Based Automated Access Control

An intelligent gate automation system that combines **Computer Vision**, **Optical Character Recognition (OCR)**, and **IoT** to provide secure and automated access control.

The system authenticates users by verifying both **facial identity** and **vehicle license plates** before granting access. Once authentication is successful, an **Arduino Uno** controls the gate mechanism automatically. Unauthorized access attempts are logged for monitoring and security.

> **Achievement:** This project was developed as our third-year minor project and was awarded **Second Runner-Up** at a national-level Hardware Hackathon.

## Project Overview

Traditional gate security systems often rely on manual verification or single-factor authentication. This project introduces a smart access control solution that combines facial recognition and license plate recognition to automate the authentication process.

The system performs real-time image processing using OpenCV, extracts license plate text using EasyOCR, compares detected identities against authorized records, and communicates with an Arduino Uno to control the gate.

## Features

- Face detection using Haar Cascade Classifier
- Vehicle detection and license plate recognition
- OCR-based license plate text extraction using EasyOCR
- Automatic gate control through Arduino Uno
- Logging of detected license plates and access history
- Real-time processing using OpenCV

## Technologies Used

### Programming Languages

- Python
- Arduino (C/C++)

### Computer Vision

- OpenCV
- Haar Cascade Classifiers

### OCR

- EasyOCR

### Hardware

- Arduino Uno
- USB Camera
- Servo Motor

### Communication

- Serial Communication (Python ↔ Arduino)

## System Workflow

1. Camera captures live video.
2. The system detects the driver's face.
3. Vehicle detection identifies the license plate region.
4. EasyOCR extracts the license plate text.
5. Face and license plate are verified against the authorized database.
6. If authentication succeeds:
   - Arduino receives the signal.
   - The gate opens automatically.
7. If authentication fails:
   - Access is denied.
   - Detection information is recorded for monitoring.

## How to Run

### Clone the repository

```bash
git clone https://github.com/yourusername/Smart-Gate-Computer-Vision-IoT.git
```

### Install dependencies

```bash
pip install -r Python/requirements.txt
```

### Connect Arduino

Upload the Arduino sketch located in:

```
Arduino/
```

### Run the application

```bash
python Python/smart_gate.py
```

## Key Functionalities

- Real-time face detection
- License plate detection
- Optical Character Recognition (OCR)
- Authorized user verification
- Automated gate control
- Detection logging
- Serial communication with Arduino

## Future Improvements

- Deep learning-based face recognition for improved accuracy
- RFID integration for multi-factor authentication
- Cloud-based access log management
- Web dashboard for monitoring
- Mobile notification system
- Support for multiple cameras
- Database integration using MySQL or PostgreSQL

## Learning Outcomes

Through this project, we gained practical experience in:

- Computer Vision using OpenCV
- Optical Character Recognition
- Python-Arduino serial communication
- IoT-based automation
- Image processing techniques
- Hardware and software integration
- Team-based engineering project development

## License

This project is licensed under the MIT License.

### Contributors

Developed as a third-year minor project by:

- **Stuti Acharya**
- **Simran Dhakal**
- **Shraddha Bhattarai**
- **Arati Shrestha**

> *An intelligent access control system that combines Computer Vision and IoT to enhance security through automated authentication.*
