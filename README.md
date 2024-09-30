# Real-time Face Detection with OpenCV
This project implements **real-time face detection** using OpenCV. It captures video from a webcam and processes each frame to detect faces, displaying bounding boxes around them.

## Table of Contents
- [Project Overview](#project-overview)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Command-line Options](#command-line-options)
- [Dependencies](#dependencies)
- [Contributing](#contributing)
- [License](#license)

## Project Overview

This application utilizes OpenCV’s Haar cascade classifier to detect human faces in real-time. It captures video streams from the webcam, detecting and drawing bounding boxes around any detected faces. The project is ideal for beginners in computer vision or anyone looking to implement basic face detection.

## Features
- **Face Detection**: Detects and tracks human faces in real-time using Haar cascades.
- **Eye Detection**: Detects eyes within detected faces.
- **Body Detection**: Optionally detects human bodies using a HOG descriptor and SVM-based detector.
- **Bounding Boxes**: Displays bounding boxes around detected faces, eyes, and bodies.
- **Command-line Options**: Easily enable or disable face and body detection via command-line flags.

## Installation
1. **Clone the repository**:
   ```bash
   git clone https://github.com/ndleah/python-mini-project.git
   cd python-mini-project/Face_Recognition
   ```
2. **Install the required packages**:
   Make sure you have Python installed and then install OpenCV:
   ```bash
   pip install opencv-python
   ```
## Usage
Run the script with the following commands:
- For face and eye detection:
  ```bash
  python your_script_name.py --face
  ```
- For body detection:
  ```bash
  python your_script_name.py --body
  ```
Press `q` to exit the video stream.

## How It Works

- **Haar Cascade Classifiers**: OpenCV’s pre-trained Haar cascades are used for face and eye detection.
- **HOG (Histogram of Oriented Gradients)**: For body detection, a HOG descriptor along with a pre-trained SVM detector is used.

When the camera is active:
- Frames are captured from the webcam.
- If face detection is enabled, the program searches for faces and eyes in each frame, drawing bounding boxes around detected faces and eyes.
- If body detection is enabled, the program searches for human bodies in each frame and displays bounding boxes around detected bodies.

## Dependencies

- **Python 3.x**
- **OpenCV**: For image processing and real-time object detection.
- **argparse**: For handling command-line options.

## Contributing

Contributions are welcome! If you have suggestions or improvements, feel free to create a pull request.

### Steps to Contribute
1. Fork the repository.
2. Create a new branch:
   ```bash
   git checkout -b your-feature-branch
   ```
3. Make your changes and commit them:
   ```bash
   git commit -m "Your descriptive commit message"
   ```
4. Push to your branch:
   ```bash
   git push origin your-feature-branch
   ```
5. Open a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.