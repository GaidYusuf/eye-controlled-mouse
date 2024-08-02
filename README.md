# Eye Controlled Mouse

This project demonstrates how to create an eye-controlled mouse using Python, OpenCV, Mediapipe, and PyAutoGUI. By tracking the movement of your eyes, you can control the mouse cursor on your screen. This project highlights the potential of computer vision for innovative human-computer interactions.

## Features

- **Eye Tracking:** Control the mouse cursor based on eye movements.
- **Blink Detection:** Simulate a mouse click when a blink is detected.
- **Click Simulation**: Simulates a mouse click when a blink or specific eye movement is detected.

## Requirements

- Python 3.x
- OpenCV
- Mediapipe
- PyAutoGUI

## Installation

1. **Clone the Repository:**

    ```bash
    git clone https://github.com/yourusername/eye-controlled-mouse.git
    cd eye-controlled-mouse
    ```

2. **Install the Required Libraries:**

    ```bash
    pip install opencv-python mediapipe pyautogui numpy
    ```

## Usage

1. **Run the Script:**

    ```bash
    python eye_controlled_mouse.py
    ```

2. **Instructions:**

    - Ensure your webcam is connected and functional.
    - Position yourself in front of the webcam.
    - The script will start tracking your eye movements.
    - The cursor will follow your eye movements, and a blink will simulate a mouse click.
    - Press `q` to exit the application.

## Code Overview

The main components of the code are:

1. **Setting up the Environment:**
   - Initializes the webcam and libraries.

2. **Capturing Video from Webcam:**
   - Captures frames from the webcam for processing.

3. **Detecting Facial Landmarks:**
   - Uses Mediapipe to detect facial landmarks, focusing on the eyes.

4. **Tracking Eye Movement:**
   - Calculates the position of the eyes and moves the mouse cursor accordingly.

5. **Interacting with the Screen:**
   - Detects blinks (by measuring the distance between two landmarks) to simulate mouse clicks.
