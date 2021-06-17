# counting_fingers
Counting fingers in a live video feed, using OpenCV and MediaPipe.

First we capture the video, and process the video, frame by frame. 

Using MediaPipe we detect the hand and its landmark points.

These landmarks are connected which you see in form of green skeleton, when it detects hand.

The x and y-coordinates of these landmarks together with their IDs gets saved in "results" object.

Using multi_hand_landmarks method on results, gives us the landmarks, which we save in a list named "lmlist"

The algorithm then checks for relative position of finger tips landmarks to the other landmarks in finger. 

This tells us whether it was open or closed. And thus it counts the total number of open fingers.

As you can see in the sample video the detection and finger counting is spontaneous.
