# EROSION-AND-DILATION

## Aim
To implement Erosion and Dilation using Python and OpenCV.
## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
<br>


### Step2:
<br>

### Step3:
<br>

### Step4:
<br>

### Step5:
<br>

 
## Program:

``` Python
# Import the necessary packages

import cv2
import numpy as np


# Create the Text using cv2.putText
img1=np.zeros((100,400),dtype="uint8")
font=cv2.FONT_HERSHEY_PLAIN
cv2.putText(img1,"PRAVEEN-S",(5,70),font,2,(255),5,cv2.LINE_AA)
cv2.imshow("image",img1)
cv2.waitKey(0)


# Create the structuring element

kernel=np.ones((5,5),np.uint8)
kernel1=cv2.getStructuringElement(cv2.MORPH_CROSS,(7,7))


# Erode the image

cv2.erode(img1, kernel)
image_erode = cv2.erode(img1,kernel1)
cv2.imshow("Praveen S-212222240077",image_erode)
cv2.waitKey(0)

# Dilate the image
image_dilatel=cv2.dilate(img1,kernel1)
cv2.imshow("Praveen S-212222240077",image_dilatel)
cv2.waitKey(0)




```
## Output:

### Display the input Image
<br>
<br>

![image](https://github.com/praveenst13/EROSION-AND-DILATION/assets/118787793/b8965373-6225-4b58-a8fa-0eb45d8b3d5b)

<br>
<br>
<br>
<br>

### Display the Eroded Image
<br>
<br>
<br>

![image](https://github.com/praveenst13/EROSION-AND-DILATION/assets/118787793/d46a495f-9e61-404f-b1b9-cdd9da2946c1)

<br>
<br>
<br>

### Display the Dilated Image
<br>
<br>
<br>

![image](https://github.com/praveenst13/EROSION-AND-DILATION/assets/118787793/5e999ea7-a0e3-45c9-b45e-1fea81868900)

<br>
<br>
<br>

## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
