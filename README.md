# Webcam Capture Application

## Description
This is a simple Python application that captures video from your computer's webcam and displays it in real-time. The program uses OpenCV (cv2) library to access and display the webcam feed.

## Requirements
- Python 3
- OpenCV (cv2) library

## Installation
1. Make sure you have Python installed on your system
2. Install OpenCV using pip:
```bash
pip install opencv-python
```

## Usage
1. Run the program:
```bash
python main.py
```
2. A window will open showing the live feed from your webcam
3. Press the 'ESC' key (key code 27) to exit the program

## How it Works
1. The program initializes the webcam using `cv2.VideoCapture(0)`
2. It enters a continuous loop that:
   - Captures frames from the webcam
   - Displays the frames in a window titled "Capture from Webcam"
3. When ESC is pressed, the program:
   - Breaks the loop
   - Releases the webcam
   - Closes all OpenCV windows

## Notes
- Make sure your computer has a working webcam
- The program uses webcam index 0 (default webcam)
- If you have multiple cameras, you can change the index in `VideoCapture(0)` to use a different camera
