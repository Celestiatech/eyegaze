# Eye Tracking System

This project implements an eye tracking system using OpenCV and Haar cascades for face and eye detection. The system captures video from the webcam, detects faces and eyes, and displays the results in real-time.

## Project Structure

```
eye-tracking-system
├── src
│   ├── eye_tracking.py          # Main logic for the eye tracking system
│   ├── utils
│   │   └── __init__.py         # Utility functions for the eye tracking system
│   └── models
│       └── haarcascades
│           ├── haarcascade_eye.xml                # Haar cascade for eye detection
│           └── haarcascade_frontalface_default.xml # Haar cascade for face detection
├── requirements.txt             # Project dependencies
├── .gitignore                   # Files and directories to ignore by Git
└── README.md                    # Documentation for the project
```

## Installation

1. Clone the repository:
   ```
   git clone <repository-url>
   cd eye-tracking-system
   ```

2. Install the required dependencies:
   ```
   pip install -r requirements.txt
   ```

## Usage

1. Ensure your webcam is connected and accessible.
2. Run the eye tracking script:
   ```
   python src/eye_tracking.py
   ```
3. The application will open a window displaying the video feed with detected faces and eyes highlighted. Press 'q' to exit the application.

## Contributing

Contributions are welcome! Please feel free to submit a pull request or open an issue for any suggestions or improvements.

## License

This project is licensed under the MIT License. See the LICENSE file for more details.