# Invisible Keyboard

A real-time contactless virtual keyboard that allows users to type using hand gestures captured through a webcam. The system uses hand landmark detection to track the user's index finger and thumb, enabling key selection through a pinch gesture. It also supports voice typing through speech recognition.

## Project Overview

Invisible Keyboard is a computer vision-based virtual keyboard designed to provide a touch-free typing interface.

The webcam captures the user's hand movements, and MediaPipe detects the hand landmarks. The index finger landmark is used to determine the key being pointed at, while the distance between the index finger and thumb is used to detect a pinch gesture. When the user performs the pinch gesture over a virtual key, the corresponding key is selected and the character is added to the text display.

The system also includes a microphone-based voice typing feature, allowing users to enter text through speech.

## Features

- Real-time hand tracking using MediaPipe
- Index finger-based key positioning
- Pinch gesture for key selection
- Virtual QWERTY keyboard
- Space, Backspace, Clear, and Microphone controls
- Voice typing using SpeechRecognition
- Real-time text display
- Keyboard click sound feedback
- FPS monitoring
- Webcam-based contactless interaction

## Technologies Used

- Python
- OpenCV
- MediaPipe
- NumPy
- SpeechRecognition
- PyAudio
- Winsound
- Jupyter Notebook

## How It Works

1. The webcam captures the user's hand movements in real time.
2. MediaPipe detects and tracks the hand landmarks.
3. The index finger landmark is used to determine the key being pointed at.
4. The distance between the index finger and thumb is calculated.
5. When the distance falls below the defined threshold, a pinch gesture is detected.
6. If the index finger is positioned over a keyboard button during the pinch gesture, that key is selected.
7. The selected character is added to the displayed text.
8. Special controls such as Space, Backspace, and Clear perform their respective operations.
9. The Microphone button starts voice recognition and adds the recognized speech to the text.



## Installation

### 1. Clone the Repository

```bash
git clone https://github.com/thanha26/Invisible_Keyboard.git
cd Invisible_Keyboard
```

### 2. Create a Virtual Environment

```bash
python -m venv venv
```

### 3. Activate the Virtual Environment

For Windows:

```bash
venv\Scripts\activate
```

### 4. Install Dependencies

```bash
pip install opencv-python numpy mediapipe SpeechRecognition PyAudio
```

## Running the Project

Open the Jupyter Notebook:

```bash
jupyter notebook keyboard.ipynb
```

Run the notebook cells and allow access to the webcam and microphone when prompted.

## Controls

| Control | Function |
|---|---|
| Alphabet Keys | Enter characters |
| SPACE | Insert a space |
| BACK | Delete the last character |
| CLEAR | Clear the complete text |
| MIC | Start voice typing |
| Pinch Gesture | Select a key |

## Future Improvements

- Improve gesture recognition accuracy
- Add customizable keyboard layouts
- Support additional languages
- Improve voice recognition handling
- Add configurable gesture thresholds
- Develop a standalone desktop application

## Author

Thanha Shajahan

## License

This project is intended for educational and portfolio purposes.
