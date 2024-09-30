# Real-time Face, Eye, and Body Detection

This project implements real-time face, eye, and body detection using OpenCV. The application captures video from a webcam and processes the frames to detect and display bounding boxes around detected faces, eyes, and bodies.

## Table of Contents
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Features
- Detects faces in real-time using Haar cascades.
- Detects eyes within the face region.
- Detects full bodies using HOG-based human detector.
- Displays bounding boxes and labels for detected faces, eyes, and bodies.
- Command-line options to enable or disable face and body detection.

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
