# BlinkGuard-SonicAlert

1. Defines a function eye_aspect_ratio(eye) that calculates the eye aspect ratio (EAR) using the Euclidean distances between eye landmarks.
2. Defines a threshold (thresh) and a frame check value (frame_check), which determine the conditions for triggering an alert.
3. Uses the dlib face detector to identify faces in the webcam feed.
   Applies a shape predictor model ("shape_predictor_68_face_landmarks (1).dat") to detect facial landmarks.
   Extracts the left and right eye regions from the detected facial landmarks.
4. Calculates the EAR for both eyes and computes the average.
   Draws contours around the eyes on the frame.
5. If the calculated EAR falls below the defined threshold, it indicates potential drowsiness.
6. The script runs until the user presses the 'q' key, at which point the script ends, and the video window is closed.
