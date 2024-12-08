# **Hand-Controlled Computer Volume**

This project uses computer vision and hand tracking to create a real-time system for controlling audio volume through intuitive hand gestures. By detecting the relative positions of fingers, it allows users to adjust volume without touching their devices. The application is developed in Python using OpenCV, MediaPipe, and Pycaw.

---

## **Features**
- **Hand Tracking**: Identifies and tracks key landmarks of the hand using MediaPipe.
- **Volume Control**: Dynamically adjusts the system's audio volume based on the distance between the thumb and index finger.
- **Real-time Visual Feedback**: Displays lines, circles, and text on the video feed to provide immediate feedback about gesture recognition.
- **Frame Rate Display**: Monitors and displays the current FPS of the application for performance tracking.

---

## **Technologies Used**
- **OpenCV**: For video capture and image processing.
- **MediaPipe**: For reliable and efficient hand tracking.
- **PyCaw**: To interface with the system's audio settings and control volume.
- **NumPy**: For mathematical calculations and data manipulation.

---

## **How It Works**
1. A webcam captures the user’s hand movements in real time.
2. MediaPipe detects the hand landmarks, including the thumb and index finger.
3. The Euclidean distance between the thumb and index finger is calculated.
4. This distance is mapped to a range of system audio volume values and applied using Pycaw.
5. Real-time feedback, such as a line connecting the fingers and volume percentage, is displayed on the video feed.

---

## **Prerequisites**
- Python 3.7 or later
- A webcam for video capture
- Required Python libraries (listed in `Technologies Used`)

---

## **Future Enhancements**
- Adding gesture-based support for media controls (e.g., play, pause, skip tracks).
- Extending support for multi-hand interactions.
- Proportional Volume Control (Planned): Adjust the system volume based on the relative size of the hand in the camera frame, ensuring consistent control regardless of the hand's distance from the camera.

---

Feel free to fork, star, or contribute to this project.
