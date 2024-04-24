# HandDino: Hand Gesture Control for Chrome's Dinosaur Game

**HandDino** is an innovative project that leverages computer vision to control Google Chrome's popular Dinosaur game using hand movements. This application uses OpenCV to recognize hand gestures and `pyautogui` to simulate keyboard presses, allowing you to play the game without physical contact with your keyboard.

## Features

- **Gesture Recognition**: Control the dinosaur with simple hand movements.
- **Real-time Interaction**: Play the Chrome Dinosaur game in real-time using your webcam.
- **Customizable Settings**: Adjust HSV values to match your ambient lighting conditions for optimal gesture recognition.

## Packages Required

- **OpenCV** (`cv2`): For image processing and gesture recognition.
- **NumPy**: For handling high-level mathematical operations.
- **Math**: For performing basic mathematical calculations.
- **PyAutoGUI**: For simulating keyboard inputs based on gestures detected.

## Installation

Before running the program, ensure you have the necessary packages installed:

```bash
pip install opencv-python numpy pyautogui
```

## Execution

To start controlling the dinosaur game with hand gestures, follow these steps:

1. **Run the Program**: Execute the main script with Python.
   ```bash
   python handdino.py
   ```
2. **Open the Game**: Go to `chrome://dino` in Google Chrome.
3. **Position Your Hand**: Keep your hand within the visible rectangle on the webcam feed to start controlling the game.

## Configuration

### Tests and Controls

- **Lighting Conditions**: You may need to adjust the HSV values in the script to better suit your current lighting conditions for more accurate gesture recognition.

### Customizing HSV Values

To modify the HSV settings, open `handdino.py` and locate the section where the HSV thresholds are set. Adjust these values to increase or decrease sensitivity to your environment's lighting:

```python
# Example of HSV adjustment
lower_hsv = np.array([0, 48, 80])
upper_hsv = np.array([20, 255, 255])
```

## Contribution

Contributions are welcome! If you have suggestions or improvements, please fork the repository and submit a pull request. You can also open an issue if you find bugs or have feature requests.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

## Contact

- **WebSite**: [Wajoud H Noorani](https://wajoudnoorani.com/)

Feel free to reach out if you have any questions or suggestions!
