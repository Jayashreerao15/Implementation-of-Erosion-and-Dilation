# Implementation-of-Erosion-and-Dilation
## Aim
To implement Erosion and Dilation using Python and OpenCV.
## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
Import the necessary packages.
### Step2:
Create the Text using cv2.putText.
### Step3:
Create the structuring element.
### Step4:
Erode and Dilate the image.
### Step5:
End Program.
## Program:
``` Python
# Developed By   : Jayashree Rao
# Register Number: 212220230023

# Import the necessary packages
import cv2
import numpy as np
import matplotlib.pyplot as plt

# Create the Text using cv2.putText
img1 = np.zeros((100,270), dtype = 'uint8')
font = cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(img1,'Aishree',(5,70), font, 2,(255),5,cv2.LINE_AA)
plt.imshow(img1,'gray')

# Create the structuring element
cv2.erode(img1, kernel)
kernel = cv2.getStructuringElement(cv2.MORPH_CROSS,(7,7))

# Erode the image
image_erode1 = cv2.erode(img1,kernel)
plt.imshow(image_erode1, 'gray')

# Dilate the image
image_dilate1 = cv2.dilate(img1, kernel)
plt.imshow(image_dilate1, 'gray')
```
## Output:
### Display the input Image
![image](https://user-images.githubusercontent.com/70213227/171025645-d3c06a78-fe13-461e-91b8-e88176d53f85.png)
### Display the Eroded Image
![image](https://user-images.githubusercontent.com/70213227/171025695-f7e1f881-5e61-4bfc-9cca-4c65e2aa5b9f.png)
### Display the Dilated Image
![image](https://user-images.githubusercontent.com/70213227/171025732-d5975a9c-df9f-4923-962f-e582023bb084.png)

## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
