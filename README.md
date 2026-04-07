# ✋ HandSensor

Control your computer's mouse using hand gestures detected through your webcam — no physical mouse needed.

---

## Quick Start

```bash
git clone https://github.com/Shin-Ryujin-korea-hangug/HandSensor
cd HandSensor
pip install opencv-python numpy pyautogui
python3 main.py
```

> Make sure your webcam is connected before running.

---

## How It Works

The program uses your webcam to detect hand landmarks in real time. Depending on which fingers you raise, it maps your hand movements to mouse actions.

### Gestures

| Gesture | Action | How |
|---|---|---|
| ☝️ Index finger up | **Move** the cursor | Raise only your index finger; the cursor follows its position |
| ✌️ Index + middle fingers up | **Click** | Raise both fingers, then bring them close together (< 40 px apart) |

### Visual Feedback

- A **rectangle** on the webcam feed shows the active detection area.
- A **circle** on your fingertip indicates the tracked position in move mode.
- A second **circle** appears when a click is registered.

---

## Requirements

- Python 3
- Webcam
- Dependencies: `opencv-python`, `numpy`, `pyautogui`

---

## Notes

- You can adjust detection parameters and thresholds directly in the source code to fit your setup.
- Contributions and feature additions are welcome.
