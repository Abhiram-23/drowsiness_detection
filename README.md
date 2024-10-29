# Drowsiness Detection Application

## Overview

This project implements a drowsiness detection application using OpenCV's Haar cascades to detect faces and eyes from a video feed. The application captures video input through a webcam and identifies when a person may be drowsy by analyzing facial features in real time.

## Features

- Real-time face and eye detection using Haar cascades.
- Live video feed from the webcam.
- Visual feedback with rectangles drawn around detected faces and eyes.
- Simple user interface, ending the session with a keypress.

## Requirements

To run this application, ensure you have the following packages installed:

- Python 3.x
- OpenCV
- NumPy
- Dlib
- Pygame
- Imutils
- SciPy

### Package Versions

The following versions are recommended for compatibility:

```
numpy==1.15.2
dlib==19.16.0
pygame==1.9.4
imutils==0.5.1
opencv_python==3.4.3.18
scipy==1.1.0
```

## Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/Abhiram-23/drowsiness_detection.git
   cd drowsiness_detection
   ```

2. **Install the required packages**:
   You can install the necessary packages using pip:
   ```bash
   pip install -r requirements.txt
   ```

3. **Download Haar Cascade Files**:
   Ensure you have the Haar cascade files (`haarcascade_frontalface_default.xml` and `haarcascade_eye.xml`) in a folder named `haarcascades` within the project directory.

## Usage

1. **Run the Application**:
   Execute the script to start the drowsiness detection application:
   ```bash
   python drowsiness_detection.py
   ```

2. **Control the Application**:
   - The application will start displaying the webcam feed.
   - Press `q` to exit the application.

## Implementation Details

- **Face Detection**: The application uses the `haarcascade_frontalface_default.xml` for face detection.
- **Eye Detection**: The `haarcascade_eye.xml` is utilized to detect eyes within the detected face region.
- **Real-Time Processing**: The video feed is processed frame by frame, and rectangles are drawn around detected faces and eyes to provide visual feedback.

## Potential Improvements

- Integrate additional algorithms to assess drowsiness more effectively (e.g., monitoring eye closure duration).
- Implement alerts or notifications when drowsiness is detected.
- Optimize the detection speed and accuracy for better performance.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [OpenCV](https://opencv.org/) for the computer vision library.
- The creators of the Haar cascade classifiers used in this application.
