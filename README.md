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


# Eye Gaze Tracking with a Web Camera

## **Project Overview**
This project enables real-time eye gaze tracking using a standard web camera. It utilizes OpenCV, Dlib, and MediaPipe for facial and eye detection, along with Python for implementation.

---

## **System Requirements**
- **OS:** Ubuntu 20.04 or later (Recommended: WSL2 for Windows users)
- **Python Version:** 3.8 or later
- **Hardware:** Webcam-enabled PC

---

## **Installation & Setup Guide**

### **Step 1: Update System Packages**
```bash
sudo apt update && sudo apt upgrade -y
```

### **Step 2: Install Dependencies**
```bash
sudo apt install python3 python3-pip python3-venv -y
```

### **Step 3: Create & Activate Virtual Environment**
```bash
python3 -m venv eyegaze_env
source eyegaze_env/bin/activate
```

### **Step 4: Install Required Python Packages**
```bash
pip install opencv-python opencv-python-headless dlib mediapipe numpy
```

### **Step 5: Clone the Repository**
```bash
git clone https://github.com/Celestiatech/eyegaze.git
cd eyegaze
```

### **Step 6: Run the Eye Tracking Script**
```bash
python eye_tracking.py
```

---

## **Troubleshooting**
### **1. OpenCV Module Not Found**
```bash
pip install --upgrade opencv-python opencv-python-headless
```

### **2. Dlib Compilation Issues**
```bash
sudo apt install cmake build-essential -y
pip install dlib
```

### **3. Systemd Errors in WSL**
If using WSL, enable systemd:
```bash
sudo nano /etc/wsl.conf
```
Add the following lines:
```ini
[boot]
systemd=true
```
Then restart WSL:
```powershell
wsl --shutdown
```

---

## **Credits**
Developed by [Your Name] for [Client Name].

---

## **License**
This project is open-source under the MIT License.

