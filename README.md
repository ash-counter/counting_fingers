# Counting_fingers
<br>
Counting fingers in a live video feed, using OpenCV and MediaPipe.
<br>
First we capture the video, and process the video, frame by frame. 
<br>
Using MediaPipe we detect the hand and its landmark points(red dots).
<br>
These landmarks are connected which you see in form of green skeleton, when it detects hand.
<br>
The x and y-coordinates of these landmarks together with their IDs gets saved in "results" object.
<br>
Using multi_hand_landmarks method on results, gives us the landmarks, which we save in a list named "lmlist"
<br>
The algorithm then checks for relative position of finger tips landmarks to the other landmarks in finger. 
<br>
As you can see in the demonstration video the detection and finger counting is spontaneous.

# Demonstration 
<img width="600px" src="https://github.com/ash-counter/counting_fingers/blob/main/Final_output.png">
