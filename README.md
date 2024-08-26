# Women Surveillance System

## Overview

The Women Surveillance System is designed to analyze real-time CCTV footage to ensure the safety of women. This project includes various features such as sending alerts to concerned authorities when a woman is alone at night or surrounded by suspicious elements. The system uses facial emotion analysis and multiple technologies to assess safety and generate alerts.

## Features

- **Object Detection**: Uses YOLO for real-time detection of persons.
- **Face Cropping & Gender Classification**: Crops faces and classifies gender using a transformer pipeline.
- **Alert System**: Sends alerts via a Telegram bot when a woman is alone at night or surrounded by unnecessary elements.
- **Emotion & Pose Detection**: Utilizes MediaPipe Holistic for detecting facial emotions and poses.
- **Distance Calculation**: Calculates the distance between the woman and nearby individuals to determine potential threats.
- **Tracking**: Employs centroid tracking for speed and movement analysis.

## Installation

1. **Clone the Repository**

   ```bash
   git clone https://github.com/ShubhamNiranjan/Surveillence_system.git
