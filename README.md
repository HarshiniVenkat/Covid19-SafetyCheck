# Covid19-SafetyCheck
* SafetyCheck is a social distance monitoring system to ensure safety standards for Covid19 is met using YOLO object detection and centroid distance evaluation. 
* This application uses pixel distance detection which varies for each user system.
* Safe people are enclosed in a green boundingbox while those at risk are enclosed in a red boundingbox.
* The application also displays the count of people who are at exposure risk.

## How to run the Application 
1. Clone the repository

2. If GPU is utilised make changes in safetycheck/safetycheck_config.py file and set `USE_GPU = TRUE`

3. If webcam is used, make changes in safetycheck.ipynb file and set `vs = cv2.VideoCapture(0)` and change the `MIN_DISTANCE = <ENTER PREFERRED DISTANCE>` in the safetycheck_congif.py file according to your need.

4. If input video is used, make changes in safetycheck.ipynb file and set `vs = cv2.VideoCapture("<PATH TO INPUT FILE>")` and change the `MIN_DISTANCE = <ENTER PREFERRED DISTANCE>` in the safetycheck_congif.py file according to your need.

5. For saving the result, mention the path to store your output file. Set `output = "<PATH TO SAVE FILE>"` in safetycheck.ipynb

## Demonstration
SafetyCheck using Webcam:

![alt text][vid]

[vid]: https://github.com/HarshiniVenkat/Covid19-SafetyCheck/blob/master/final.gif "SafetyCheck"

SafetyCheck on Input Video: 

![alt text][logo]

[logo]: https://github.com/HarshiniVenkat/Covid19-SafetyCheck/blob/master/output.avi "output File"
