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

 **Clone the Repository**

   ```bash
   git clone https://github.com/ShubhamNiranjan/Surveillence_system.git
 **Create and Activate Virtual Environment**

   - Using `venv`:
     ```bash
     python -m venv env
     env\Scripts\activate
     ```

   - Using `conda`:
     ```bash
     conda create -n env
     conda activate env
     ```

 **Install Requirements**

   ```bash
   pip install -r requirements.txt
## Running the Project

 **Run the Main Script**

   ```bash
   python main.py
## Testing

- Two video files are provided in the repository to help you test the system.
- To use your own video files, modify the `cv2.VideoCapture(0)` command in the code to reference the path of your video file.
- For webcam input, ensure the argument for `cv2.VideoCapture` is set to `0` to use the default webcam.
## Future Enhancements

- **Violence Detection**: Develop and integrate algorithms to identify and alert for violent behavior.
- **Fire Detection**: Add functionality to detect fire in the footage and notify authorities.
- **Fall Detection**: Implement features to detect falls and send alerts for immediate assistance.
- **Super-Resolution**: Enhance the resolution of blurry CCTV images to improve detection and reduce errors.

