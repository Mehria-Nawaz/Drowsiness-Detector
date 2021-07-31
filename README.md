# Drowsiness-Detector
Drowsiness detector is a detector which helps to detect if a person is drowsy. It is a very useful detector as many road accidents are caused due to sleep driving at night. It is natural that a person will feel sleepy at night, hence people who drive trucks and heavy load vehicle specially at night feel sleepy and tend to drowse which result in different types of car accidents. Hence, we have made an effort to help them and prevent these accidents and make their family members feel relaxed and not worry.

## ABOUT THE PROJECT
	The project is easy to read and compatible to run after some prerequisites. First we should know about eye aspect ratio.
	Each eye is represented by 6 (x, y)-coordinates, starting at the left-corner of the eye (as if you were looking at the person), and then working clockwise around the remainder of the region.
 	 The numerator of the equation computes the distance between the vertical eye landmarks while the denominator computes the distance between horizontal eye landmarks, weighting the denominator appropriately since there is only one set of horizontal points but two sets of vertical points.
	The ear is an important concept because it helps in predicting whether the eye is closed, open or there is a blink. The eye aspect ratio is approximately constant while the eye is open, but will rapidly fall to zero when a blink is taking place and becomes nearly zero when the eye closes.

#### PREREQUISITES
	
	Anaconda Navigator 
	Then we need to download some packages, those are:
	opencv
	dlib
	imutils
	playsound
	You need to download an alarm sound of format .wav and name it alarm- and the shape predictor file named shape_predictor_68_face_landmarks.dat

#### HOW IT WORKS
	This project uses the 68 coordinate system of detecting the parts of the face. We have extracted the coordinates of eye and using the eye aspect ratio concept build a drowsiness detector.
	First the webcam launches and our eyes are detected by a green convex hull and the ear is shown simultaneously. As soon as the eyes ear goes below a certain value the alarm rings and stops ringing when the eyes are open again.
	Hence, this would help in predicting the drowsiness of a person and help to reduce accidents.

