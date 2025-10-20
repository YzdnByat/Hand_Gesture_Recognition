# Hand Gesture Recognition with Mediapipe & LSTM

This project implements a **real-time hand gesture recognition system** using **Mediapipe** for hand landmark detection and an **LSTM deep learning model** for sequence classification.  
The system recognizes five common gestures and maps them to multimedia control actions such as volume adjustment, video navigation, and play/pause.

---

## ✨ Features
- Extracts **21 hand landmarks** (x, y, z coordinates) from each video frame using Mediapipe.
- Builds temporal sequences of 30 frames to capture motion dynamics.
- Trains a **stacked LSTM network** with dropout and dense layers for gesture classification.
- Achieves **97–98% accuracy** on validation sets.
- Real-time **inference pipeline** with webcam input.
- Uses **PyAutoGUI** to trigger system commands:
  - 👍 Thumbs Up → Volume Up  
  - 👎 Thumbs Down → Volume Down  
  - 👋 Left Swipe → Rewind video  
  - 👉 Right Swipe → Forward video  
  - ✊ Fist (Stop gesture) → Play/Pause  

---

## 📂 Project Structure
Hand_Gesture_Recognition/
│
├── Hand_Gesture_Recognition.ipynb # Main Jupyter Notebook
├── Hand_Gesture_Recognition.pdf # Full project report
├── models/ # Trained LSTM models (saved .h5 files)
├── gifs/ # Demo animations
└── README.md

