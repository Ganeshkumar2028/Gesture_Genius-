# Requisites 

* [Tkinter](https://pypi.org/project/tk-tools/) for to create graphical user interfaces (GUIs)
* [Mediapipe](https://pypi.org/project/mediapipe/) for Recognizing hand gestures
* [Autopy](https://pypi.org/project/autopy/) for pointers
* [Pydirectinput](https://pypi.org/project/PyDirectInput/) for keyboard inputs.

# Explanation

-The code is a Python script that uses the Mediapipe library to detect hand landmarks from a live video stream and then performs mouse and keyboard actions based on the hand gestures.

-The script begins by Importing the necessary libraries and initializing objects for capturing video from the webcam and for detecting hand landmarks using the Mediapipe library. 

-It also imports the Autopy library for mouse movement and the PyDirectInput library for keyboard input.

-The script then defines two functions: “handLandmarks” and “fingers”. The “handLandmarks” function takes a color image as input and returns a list of landmark coordinates for each hand that is detected in the image. 

-The “fingers” function takes the list of landmark coordinates as input and returns a list of booleans indicating whether each finger is up or down.

-The script then enters a while loop that captures video from the webcam and processes each frame to detect hand landmarks and perform mouse and keyboard actions based on the hand gestures. 

-For each frame, the script converts the color image from BGR format to RGB format, detects the hand landmarks using the “handLandmarks” function, and checks for various hand gestures using the “fingers” function.

-If the pointing finger is up and the thumb finger is down, the script moves the mouse cursor based on the position of the pointing finger. If the pointer finger is down and the thumb finger is up, the script performs a left click using the “p1.click” function. 

-If all five fingers are up, the script performs a right arrow key press using the “p1.keyDown” and “p1.keyUp” functions. If all fingers are down, the script performs a left arrow key press using the same functions.

-The code Is used to perform various actions using hand gestures, such as controlling the mouse cursor, performing mouse clicks, and keyboard actions. It can be used for various applications such as virtual presentations, gaming, and controlling devices hands-free.
