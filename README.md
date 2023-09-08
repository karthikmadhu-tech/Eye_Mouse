# Eye Tracking Mouse

Eye Tracking Mouse is a Python project that allows you to control your computer's mouse cursor using your eyes. This project uses computer vision techniques and libraries such as OpenCV, Mediapipe, and PyAutoGUI to track the movement of your eyes and simulate mouse actions, like moving the cursor and clicking.

## Requirements

Before running this project, ensure you have the following libraries installed:

- OpenCV (`cv2`)
- Mediapipe (`mediapipe`)
- PyAutoGUI (`pyautogui`)

You can install these libraries using `pip`:

```bash
pip install opencv-python-headless mediapipe pyautogui
```

## How to Use

1. Connect a webcam to your computer if it's not already connected.

2. Run the `eye_tracking_mouse.py` script.

```bash
python eye_tracking_mouse.py
```

3. A window named "Eye Mouse" will open, displaying the video feed from your webcam.

4. Look at the screen, and the program will track your eye movements.

5. Move your eyes to control the mouse cursor. The cursor will follow the movement of your eyes.

6. Blink both of your eyes (or a predefined gesture) to simulate a mouse click.

7. To exit the program, press the 'q' key while the "Eye Mouse" window is active.

## How It Works

This project uses the following libraries and techniques:

- OpenCV (`cv2`) to capture video from your webcam and display the video feed.

- Mediapipe (`mediapipe`) to detect facial landmarks, particularly the landmarks representing the eyes.

- PyAutoGUI (`pyautogui`) to control the mouse cursor and perform mouse clicks.

- The program continuously captures frames from the webcam, detects the positions of your eyes using facial landmark detection, and moves the mouse cursor accordingly.

- When you blink your eyes (or perform a predefined gesture), the program simulates a mouse click action.

## Customization

You can customize this project by adjusting the following parameters:

- Change the gesture for mouse clicking by modifying the conditions in the code.

- Adjust the delay after clicking (`pyautogui.sleep(1)`) to change the duration of the mouse click.

- Experiment with different facial landmark indices to fine-tune the tracking for your specific use case.

## Troubleshooting

If you encounter any issues or want to improve the accuracy of eye tracking, consider experimenting with different facial landmark models or adjusting the code to suit your needs.
