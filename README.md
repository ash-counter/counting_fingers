# counting_fingers
Counting fingers in a live video feed, using OpenCV and MediaPipe.
First we capture the video, and process the video, frame by frame. 
Using MediaPipe we detect the hand and its landmark points.
These landmarks are connected which you see in form of green skeleton, when it detects hand.
The x and y-coordinates of these landmarks together with their IDs gets 
