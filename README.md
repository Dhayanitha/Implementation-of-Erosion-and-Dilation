# IMPLEMENTATION OF EROSION AND DILATION
## AIM:
To implement Erosion and Dilation using Python and OpenCV.
## SOFTWARE REQUIRED:
1. Anaconda - Python 3.7
2. OpenCV
## ALGORITHM:
### Step 1:
Import the necessary packages.
### Step 2:
Create the Text using cv2.putText
### Step 3:
Create the structuring element.
### Step 4:
Erode the image.
### Step 5:
Dilate the image.

## PROGRAM:
### Developed by   : H.Dhayanitha
### Register Number: 212220230010

# Import the necessary packages
```
import cv2
import numpy as np
import matplotlib.pyplot as plt
```

# Create the Text using cv2.putText
```
img1=np.zeros((100,400),dtype='uint8')
font=cv2.FONT_ITALIC
cv2.putText(img1,'U Bhavya',(5,70),font,2,(255),5,cv2.LINE_AA)
plt.axis('off')
plt.imshow(img1)
plt.show()
```

# Create the structuring element
```
kernel=cv2.getStructuringElement(cv2.MORPH_CROSS,(9,9))
```

# Erode the image
```
image_erode1=cv2.erode(img1,kernel)
plt.axis('off')
plt.imshow(image_erode1)
plt.show()
```

# Dilate the image
```
image_dilate1=cv2.dilate(img1,kernel)
plt.axis('off')
plt.imshow(image_dilate1)
plt.show()
```

## Output:

### Display the input Image

![D1](https://user-images.githubusercontent.com/75235032/169961791-67dfb030-78ea-47e4-8f45-1304cdac4552.jpg)

### Display the Eroded Image

![D2](https://user-images.githubusercontent.com/75235032/169961831-3e7ade44-7190-422a-b54a-1bfca5161ea0.jpg)

### Display the Dilated Image

![D3](https://user-images.githubusercontent.com/75235032/169961850-13ef34a0-81e1-4f75-b318-f637d9c42422.jpg)

## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
