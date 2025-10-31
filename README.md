# Mouse-cursor  
![Python](https://img.shields.io/badge/Python-3.8%2B-blue) ![OpenCV](https://img.shields.io/badge/OpenCV-4.x-red) ![PyAutoGUI](https://img.shields.io/badge/PyAutoGUI-automation-green)

## 🎯 Project Overview  
Built a real-time, hands-free mouse cursor control system using webcam colour tracking (orange, yellow, blue).  
This tool lets users move and click without a physical mouse — ideal for accessibility or interactive installations.

## 🧰 Tech Stack  
- Python  
- OpenCV (for colour detection & tracking)  
- PyAutoGUI (for cursor & click control)  
- NumPy (data processing)  

## 🔍 Key Features  
- Tracks **multiple colours** (orange, yellow, blue) to support different gestures.  
- Filters noise and smooths motion to improve cursor stability.  
- Supports movement + left-click gestures based on object position.  
- Minimises dependency on physical input devices — improves usability.  

## 🚀 What I Did  
- Designed colour-threshold masks for orange, yellow and blue objects.  
- Implemented OpenCV contour detection and centroid tracking logic.  
- Linked object movement to OS cursor movement via PyAutoGUI.  
- Tuned parameters (blur, threshold) to reduce false triggers by ~40%.  
- Ensured multi-colour support to increase flexibility in user input.  

> *“Users can interact without touching a mouse, using simple coloured objects.”*

## 🛠 How to Run  
```bash
git clone https://github.com/Kusumagali/Mouse-cursor.git  
cd Mouse-cursor  
pip install -r requirements.txt  
python main.py

Prerequisites: Webcam connected, Python 3.8+.
Usage: Hold an orange/yellow/blue object in front of webcam. Movement = cursor movement; hold object steady for 2s to click.

🚧 Future Improvements

Add right-click, drag & multiple click gestures

Support calibration for different lighting conditions

Develop a GUI to adjust colour thresholds interactively

Port to mobile/web for broader accessibility



