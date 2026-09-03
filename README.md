
# r3ad — Hand Tracking Energy Effect 🖐️⚡

A real-time TouchDesigner piece where hand movement drives a dynamic energy/particle effect — tracked hands become the source of glowing, reactive visuals.

<img width="1357" height="840" alt="image" src="https://github.com/user-attachments/assets/8c6e36d7-240d-4576-8c14-514c2cd0d27c" />

## Overview

This project uses real-time hand tracking to drive a particle/energy visual effect in TouchDesigner. As the hand moves, [describe what happens — e.g. "particles trail from the fingertips," "an energy field pulses around the palm," "the effect intensifies with fist/open-hand gestures"]. Built as [a class project / personal exploration / performance tool / etc.].

## Requirements

- TouchDesigner **2025.33230** (or note the minimum version)
- OS: Windows
- Webcam (or other camera source used for tracking)
- Hand tracking method: [MediaPipe via Python / Kinect / Leap Motion / TDAbleton or other — specify which]
- [Any Python packages needed, e.g. `mediapipe`, `opencv-python` — list exact versions if it matters]

## Project structure

```
r3ad TouchDesigner.toe    # main project file
docs/                      # screenshots, preview gif/video
tox/                       # (if any) reusable component files
```

## Setup

1. Clone the repo:
   ```bash
   git clone https://github.com/yourusername/yourrepo.git
   ```
2. [If using MediaPipe/Python] Install dependencies:
   ```bash
   pip install mediapipe opencv-python
   ```
3. Open `r3ad TouchDesigner.toe` in TouchDesigner.
4. Make sure your webcam is connected and selected as the input device.
5. [Any other setup — e.g. "hit play on the Video Device In TOP", "run the hand tracking script from the Text DAT / Execute DAT"]

## How it works (brief)

- **Input**: [webcam → hand tracking method] extracts hand landmark positions (fingertips, palm center, etc.)
- **Mapping**: those coordinates drive [particle emitter position / noise field / GLSL shader parameters / etc.]
- **Output**: rendered as [particles / trails / glow shader] composited over [camera feed / black background / etc.]

## Controls / Usage

- Move your hand in front of the camera — the effect follows hand position in real time.
- [Any gesture controls, e.g. "open palm = effect expands," "fist = effect contracts," keyboard toggles, etc. — or remove if none]

## Notes

- [Known limitations — e.g. lighting sensitivity, tracking drops at fast movement, single-hand only]
- [Performance notes — GPU used, resolution/FPS it was built/tested at]


