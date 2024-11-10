Real-Time Face Recognition with OpenCV and DeepFace
This project performs real-time face recognition to detect and verify if a person matches any predefined reference images. Using OpenCV for capturing webcam video and DeepFace for face verification, the model displays a "MATCH!" or "NO MATCH!" message based on the results.

Overview
The primary goal of this project is to implement a real-time face recognition system that can compare live video feed images against multiple reference images. This application can be used for quick verification in various scenarios, providing an accessible introduction to facial recognition using DeepFace.

Features
Real-Time Face Detection: Captures video from a webcam feed and detects faces in each frame.
Face Verification: Compares detected faces against a list of reference images and displays live feedback.
Multithreaded Processing: Uses threading to verify faces every few frames, ensuring smooth performance.
Technologies Used
Python 3.x
OpenCV: For capturing video and displaying results.
DeepFace: For verifying faces against reference images.
Threading: For efficient frame processing in real-time.
How to Use
1.Clone the repository or download the code files.

2.Install the required libraries. You can install the dependencies with:

pip install opencv-python-headless deepface

3.Add Reference Images: Place the reference images (e.g., reference1.jpg, reference2.jpg) in the project folder. Ensure these images are named correctly and referenced in the code.

4.Run the Script:

python face_recognition.py

#Press q to exit the program.

Project Structure
real-time-face-recognition/
├── face_recognition.py         # Main Python script
├── reference1.jpg              # Reference image for face comparison
├── reference2.jpg              # Additional reference image (add as many as needed)
└── README.md                   # Project README file

Code Explanation
Capture Video: Captures video using OpenCV from the default webcam.
Face Verification: Every 30 frames, verifies if the face in the current frame matches any reference image.
Display Results: Displays "MATCH!" if a match is found, otherwise displays "NO MATCH!".
Conclusion
This project showcases the basics of real-time face verification using OpenCV and DeepFace. It’s an effective starting point for building more advanced face recognition systems and demonstrates the feasibility of real-time applications using simple models.




