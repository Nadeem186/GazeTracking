
This project is a real-time (back-end) and manual image uploading (front-end) eye gaze detection system that uses computer vision techniques to analyze where a person is looking left, right, or center directly through their webcam. It uses the dlib library for face detection and landmark prediction and processes live webcam frames using OpenCV.

The project aims to simulate behavioral cues associated with Social Anxiety Disorder (SAD). Individuals with SAD often avoid eye contact or shift their gaze frequently. By tracking such patterns live, the system can support research or assistive applications in mental health.

#  Eye Gaze Direction Detection with Dlib & OpenCV

This project detects the **eye gaze direction** (Left, Center, Right) from webcam
# Files Used

- `shape_predictor_68_face_landmarks.dat`: Pretrained Dlib model for detecting 68 facial landmarks.
- Python script (`.ipynb` or `.py`): Performs image processing, eye detection, gaze analysis, and visualization.

## How to Download the Shape Predictor (important)

You must download the **`shape_predictor_68_face_landmarks.dat`** file to use this project.

Download link:  
https://github.com/davisking/dlib-models/raw/master/shape_predictor_68_face_landmarks.dat.bz2

# Steps:
1. Download and extract the `.bz2` file and extract it.
2. Upload `shape_predictor_68_face_landmarks.dat` to your project directory (in Google Colab, use the file browser).

# How It Works
1. Face Detection: Uses Dlib's HOG-based frontal face detector.
2. Facial Landmark Detection: Loads 68-point landmarks to identify eye regions.
3. Eye Analysis:
   - Extracts left and right eye regions.
   - Applies thresholding to detect pupil position.
   - Estimates gaze direction using the center of mass.
4. Result Display: Adds text labels on images and shows the result.

# Dependencies

Install these in your Python environment or Colab:

```bash
pip install opencv-python dlib imutils matplotlib
