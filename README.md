# Eye-Tracking-Mouse: Facial Landmark Mouse Tracking

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![OpenCV](https://img.shields.io/badge/OpenCV-4.x-green.svg)
![MediaPipe](https://img.shields.io/badge/MediaPipe-Face%20Mesh-orange.svg)

Eye-Tracking-Mouse is a hands free, computer vision based mouse controller. It utilizes your webcam to map facial landmarks in realtime, allowing you to control your computer's cursor with your eyes, trigger clicks through intentional blinks, and scroll using mouth and nose gestures. 

## ✨ Features

* **Real-Time Eye Tracking:** Maps pupil movement to screen coordinates with a 9-point calibration system.
* **Smart Clicking:** Detects sustained blinks (filtering out natural blinks) to trigger left and right mouse clicks.
* **Gesture Scrolling:** Opening your mouth toggles scroll mode, allowing you to scroll pages up and down by moving your head.
* **Auto-Typing Pause:** Listens for keyboard input and automatically halts cursor movement while you are typing to prevent accidental clicks.
* **Cursor Smoothing:** Implements a smoothing factor to reduce jitter and provide fluid cursor movement.

## 🛠️ Prerequisites

Ensure you have Python 3.8 or higher installed on your system. You will also need a functional webcam.

## 🚀 Installation & Setup

1. **Clone the repository--->**

    <ins>In vscode-terminal/bash: </ins>

    ***git clone [https://github.com/frakxzo/Eye-Tracking-Mouse.git](https://github.com/frakxzo/Eye-Tracking-Mouse.git)***

     ***cd Eye-Tracking-Mouse***

2. **Install the required dependencies--->**

   <ins>It is recommended to use a virtual environment.</ins>

    ***pip install -r requirements.txt***

3. **Run the application--->**

     <ins>Terminal:</ins>

     ***python eyetrackingv7.py***


## 🎮 Usage Guide
Upon launching the script, the system will initiate a brief setup and calibration phase:

**Calibration:** Look directly at the green circles as they appear on different parts of your screen. Keep your head centered.

**Cursor Movement:** Once calibrated, look around your screen to move the cursor.

**Clicking:**  Hold your eyes closed for 0.3 seconds to trigger a click.

The system alternates between Left Click and Right Click upon successive intentional blinks.

**Scrolling:**

Open your mouth slightly to toggle "Scroll Mode".

Move your nose up or down to scroll the active window.

Close your mouth or wait 3.0 seconds to exit scroll mode.

**Typing:** Simply start typing on your keyboard. Tracking will pause automatically and resume 3.0 seconds after your last keystroke.

## 🛑 Exiting the Program
**Press the ESC key while the OpenCV window is active to safely release the camera and terminate the script.**    

## ⚠️ Note :
You may need 60fps camera for smooth experience.Also, If your setup have multiple cameras then please set the correct CAMERA_INDEX number.(by default=0)

#End of file




