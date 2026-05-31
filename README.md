 # Vision-Based Gesture-Controlled Servo Motor Positioning on Raspberry Pi Using MediaPipe and OpenCV

## Overview

This project presents a vision-based human-machine interaction system that controls the angular position of a servo motor using hand gestures. The system utilizes a Raspberry Pi, USB camera, MediaPipe, and OpenCV to detect hand landmarks in real time and translate gestures into corresponding servo motor positions.

The solution enables touchless and intuitive control without requiring wearable sensors or specialized hardware, making it suitable for robotics, automation, smart home systems, and educational applications.

---

## Features

* Real-time hand gesture recognition
* Touchless servo motor control
* MediaPipe-based hand landmark detection
* OpenCV image processing
* Raspberry Pi implementation
* Low-cost and portable setup
* Smooth and responsive servo positioning
* No wearable sensors required

---

## Hardware Requirements

* Raspberry Pi 4
* USB Camera
* SG90 Servo Motor
* Jumper Wires
* Power Supply

---

## Software Requirements

* Python 3
* OpenCV
* MediaPipe
* NumPy
* RPi.GPIO

---

## System Architecture

1. Video Acquisition using USB Camera
2. Frame Preprocessing using OpenCV
3. Hand Landmark Detection using MediaPipe
4. Gesture Recognition
5. Gesture-to-Angle Mapping
6. PWM Signal Generation
7. Servo Motor Actuation

---

## Gesture-to-Servo Mapping

| Gesture       | Servo Angle |
| ------------- | ----------- |
| Closed Fist   | 0°          |
| One Finger    | 30°         |
| Two Fingers   | 60°         |
| Three Fingers | 90°         |
| Four Fingers  | 120°        |
| Open Palm     | 150°        |

---

## Methodology

### Video Acquisition and Preprocessing

A USB camera continuously captures live video frames. OpenCV is used to resize and preprocess the images for reliable gesture detection.

### Hand Detection

MediaPipe Hands identifies and tracks 21 hand landmarks in real time.

### Gesture Recognition

Distances and angles between detected landmarks are analyzed to classify hand gestures.

### Servo Control

The recognized gesture is mapped to a predefined servo angle. Raspberry Pi GPIO generates PWM signals to position the servo accordingly.

---

## Results

* Accurate gesture recognition under normal indoor conditions
* Servo response time of approximately 200–250 ms
* Low computational overhead
* Smooth servo movement with minimal jitter
* Reliable operation across different backgrounds

### Performance Summary

| Metric                       | Performance    |
| ---------------------------- | -------------- |
| Gesture Recognition Accuracy | 80–85%         |
| Response Time                | 200–250 ms     |
| Number of Gestures           | 6              |
| Processing Platform          | Raspberry Pi 4 |

---

## Applications

* Educational Robotics
* Human-Machine Interaction Systems
* Smart Home Automation
* Assistive Technologies
* Gesture-Controlled Devices
* Interactive Learning Platforms

---

## Advantages

* Contactless operation
* Low hardware cost
* Easy deployment
* Natural user interaction
* Portable and scalable

---

## Future Scope

* Multi-servo robotic arm control
* Dynamic gesture recognition
* AI-based adaptive gesture learning
* Improved robustness under varying lighting conditions
* Integration with IoT and smart automation systems


---

## Conclusion

The project successfully demonstrates a low-cost, vision-based gesture control system capable of translating hand gestures into real-time servo motor movements. By combining Raspberry Pi, MediaPipe, and OpenCV, the system provides an intuitive and touch-free control mechanism suitable for various robotics and automation applications.
