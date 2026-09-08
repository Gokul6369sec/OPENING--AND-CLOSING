## OPENING--AND-CLOSING

### Name : GOKULAN R
### Reg No : 212224230076

## Aim
To implement Opening and Closing using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
Import the necessary packages


### Step2:
Create the Text using cv2.putText

### Step3:
Create the structuring element

### Step4:
Use Opening operation

### Step5:
Use Closing Operation
 
## Program:

```

import cv2
import numpy as np
import matplotlib.pyplot as plt
image = np.zeros((500, 500, 3), dtype=np.uint8)
font = cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(image, 'Open and Close', (100, 250), font, 1, (255, 255, 255), 2, cv2.LINE_AA)
kernel = np.ones((3, 3), np.uint8)
plt.subplot(1, 3, 1)
plt.imshow(cv2.cvtColor(image, cv2.COLOR_BGR2RGB))
plt.title("Input Image")
plt.axis('off')
plt.subplot(1, 3, 2)
plt.imshow(cv2.cvtColor(opened_image, cv2.COLOR_BGR2RGB))
plt.title("Opening Operation")
plt.axis('off')
plt.subplot(1, 3, 3)
plt.imshow(cv2.cvtColor(closed_image, cv2.COLOR_BGR2RGB))
plt.title("Closing Operation")
plt.axis('off')



```
## Output:

### Display the input Image
<img width="389" height="409" alt="image" src="https://github.com/user-attachments/assets/fa035c05-a2ad-46db-a1e9-845903ab38ca" />


### Display the result of Opening

<img width="389" height="409" alt="image" src="https://github.com/user-attachments/assets/e625cb96-9659-4d37-a225-9db3035b4d53" />


### Display the result of Closing

<img width="389" height="409" alt="image" src="https://github.com/user-attachments/assets/098bc93c-ed6f-4e8f-9f7e-37cdfefa5287" />


## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
