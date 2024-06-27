PRODIGY_ML_04

The task for the fourth project of Prodigy Infotech's Machine Learning Internship is to develop a hand gesture recognition model.  

I have used a live dataset from my own webcam. 

The project that I have done here is raising and lowering of device volume by computing the distance between the tip of the fore finger and tip of thumb. 

Attached is Jupyter notebook with code as well as documentation explaining in detail how to achieve the desired output. 

I have also attached the outputs for this particular program. 

In order to achieve the above the following steps have to be followed

Steps:

> Import necessary libraries such as open cv, mediapipe(for webcam) and pyautogui (for modifying the device volume)

> Initialize all the variables and also the webcam input.  

> Check for the presence of a hand or multiple hands on screen (program automatically uses the data produced by the first hand (pair of fore finger and thumb) appeared on field). 

> In the case of a hand present, landmark the tips of the two fingers.

> Mark the tips. (I have used a black circle)

> Compute the distance between the two landmarks for as long as the hand is in the frame.

> Formula used in computing is basic distance formula using cartesian coordinates. (square root((x2-x1)^2 + (y2-y1)^2))

> If the fingers are wide apart (say 20 pixels or more), increase volume.

> If the fingers are close together (say lesser than 20 pixels but more than 8), decrease volume.

> If the fingers completely closed together (say less than 8 pixels) break from the loop and end program (destroy all windows).

> Run the program and adjust the distance values if required. 
