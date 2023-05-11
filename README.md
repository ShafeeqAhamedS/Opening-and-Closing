# <p align="center">Opening and Closing</p>

## Aim:
To implement Opening and Closing using Python and OpenCV.

## Software Required:
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step 1:
Import the necessary packages
### Step 2:
Read the image
### Step 3:
Create the structuring element
### Step 4:
Use Opening operation
### Step 5:
Use Closing Operation
### Step 6:
Display all the output images

</br></br>
</br>
 
## Program:
Developed By   : **Shafeeq Ahamed. S**
</br>

Register Number: **212221230092**

### Import the necessary packages
```py
import cv2
import matplotlib.pyplot as plt
```

### Plot Function
```py
def plot(img):
    plt.imshow(img)
    plt.axis('off')
```
### Create the text using cv2.putText
```py
image = np.zeros((200,1150),dtype='uint8')
font=cv2.FONT_HERSHEY_SCRIPT_COMPLEX
cv2.putText(image,'Shafeeq Ahamed',(20,140),font,5,(255),3,cv2.LINE_AA)
plot(image)
```

### Create the structuring element
```py
kernel=cv2.getStructuringElement(cv2.MORPH_RECT,(5,5))
```

### Use Opening operation
```py
img1=cv2.morphologyEx(image,cv2.MORPH_OPEN,kernel)
plot(img1)
```

### Use Closing Operation
```py
img2 = cv2.morphologyEx(image,cv2.MORPH_CLOSE,kernel)
plot(img2)
```

</br></br>

## Output:

### Display the input Image
![image](https://github.com/ShafeeqAhamedS/Opening-and-Closing/assets/93427237/6384646d-469a-458d-8025-ffee6c494352)
### Display the result of Opening
![image](https://github.com/ShafeeqAhamedS/Opening-and-Closing/assets/93427237/52f4f070-b0ee-4aa4-a2cd-3c90de2e3711)
### Display the result of Closing
![image](https://github.com/ShafeeqAhamedS/Opening-and-Closing/assets/93427237/9d608a03-70b6-478a-98b3-9c2cc1c4d058)

## Result:
Thus the Opening and Closing operation is used in the image using python and OpenCV.
