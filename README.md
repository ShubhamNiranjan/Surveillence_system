<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Women Surveillance System</title>
</head>
<body>
    <h1>Women Surveillance System</h1>

    <h2>Overview</h2>
    <p>The Women Surveillance System is designed to analyze real-time CCTV footage to ensure the safety of women. This project includes various features such as sending alerts to concerned authorities when a woman is alone at night or surrounded by suspicious elements. The system uses facial emotion analysis and multiple technologies to assess safety and generate alerts.</p>

    <h2>Features</h2>
    <ul>
        <li><strong>Object Detection</strong>: Uses YOLO for real-time detection of persons.</li>
        <li><strong>Face Cropping & Gender Classification</strong>: Crops faces and classifies gender using a transformer pipeline.</li>
        <li><strong>Alert System</strong>: Sends alerts via a Telegram bot when a woman is alone at night or surrounded by unnecessary elements.</li>
        <li><strong>Emotion & Pose Detection</strong>: Utilizes MediaPipe Holistic for detecting facial emotions and poses.</li>
        <li><strong>Distance Calculation</strong>: Calculates the distance between the woman and nearby individuals to determine potential threats.</li>
        <li><strong>Tracking</strong>: Employs centroid tracking for speed and movement analysis.</li>
    </ul>

    <h2>Installation</h2>
    <ol>
        <li><strong>Clone the Repository</strong>
            <pre><code>git clone https://github.com/ShubhamNiranjan/Surveillence_system.git</code></pre>
        </li>
        <li><strong>Create and Activate Virtual Environment</strong>
            <ul>
                <li>Using <code>venv</code>:
                    <pre><code>python -m venv env
env\Scripts\activate</code></pre>
                </li>
                <li>Using <code>conda</code>:
                    <pre><code>conda create -n env
conda activate env</code></pre>
                </li>
            </ul>
        </li>
        <li><strong>Install Requirements</strong>
            <pre><code>pip install -r requirements.txt</code></pre>
        </li>
    </ol>

    <h2>Running the Project</h2>
    <ol>
        <li><strong>Run the Main Script</strong>
            <pre><code>python main.py</code></pre>
        </li>
        <li><strong>Testing</strong>
            <ul>
                <li>Two video files are provided in the repository.</li>
                <li>You can use your own video files by altering the <code>cv2.VideoCapture(0)</code> command to use a different file.</li>
                <li>For webcam input, set the argument to <code>0</code> for the default webcam.</li>
            </ul>
        </li>
    </ol>

    <h2>Future Enhancements</h2>
    <ul>
        <li><strong>Violence Detection</strong>: Implement algorithms to detect violence.</li>
        <li><strong>Fire Detection</strong>: Integrate fire detection capabilities.</li>
        <li><strong>Fall Detection</strong>: Add functionality to detect falls.</li>
        <li><strong>Super-Resolution</strong>: Improve image quality of blurry CCTV footage to reduce errors.</li>
    </ul>
</body>
</html>
