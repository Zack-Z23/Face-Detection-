# Face Detection App

A real-time face detection application built with Python and OpenCV. The app accesses your webcam feed and automatically detects and highlights faces using a pre-trained Haar Cascade Classifier — no internet connection or cloud API required.

## Features

- **Real-time detection** — processes your live webcam feed frame by frame
- **Visual highlighting** — draws bounding rectangles around every detected face
- **Offline & lightweight** — runs entirely on your machine using OpenCV's built-in Haar Cascade model
- **Simple setup** — minimal dependencies, up and running in minutes

## Tech Stack

- **Python 3.x**
- **OpenCV** (`cv2`) — computer vision and webcam capture
- **Haar Cascade Classifier** — pre-trained face detection model

## Getting Started

### Prerequisites

- Python 3.x
- pip

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/Zack-Z23/Face-Detection-.git
   cd Face-Detection-
   ```

2. Install dependencies:
   ```bash
   pip install opencv-python
   ```

### Running the App

```bash
python facedetect.py
```

A window will open showing your webcam feed. Detected faces will be outlined with rectangles in real time. Press `q` to quit.

## How It Works

The app uses OpenCV's `CascadeClassifier` loaded with the `haarcascade_frontalface_default.xml` model. Each frame from the webcam is converted to grayscale and passed through the classifier, which returns the coordinates of any detected faces. Those coordinates are then used to draw rectangles on the original colour frame before displaying it.

## Project Structure

```
Face-Detection-/
├── facedetect.py   # Main application script
└── README.md
```

## Author

Zacharias Zachariadis — [GitHub](https://github.com/Zack-Z23)
