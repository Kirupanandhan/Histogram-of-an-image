# Histogram and Histogram Equalization of an image
## Aim
To obtain a histogram for finding the frequency of pixels in an Image with pixel values ranging from 0 to 255. Also write the code using OpenCV to perform histogram equalization.

## Software Required:
Anaconda - Python 3.7

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
```python
# Developed By:
# Register Number:
import cv2
import matplotlib.pyplot as plt

# Write your code to find the histogram of gray scale image and color image channels.
import cv2
import matplotlib.pyplot as plt
gray_image=cv2.imread('5.jpeg')
color_image=cv2.imread('3.jpeg')
hist=cv2.calcHist([gray_image],[0],None,[256],[0,256])
hist1=cv2.calcHist([color_image],[1],None,[256],[0,256])
plt.imshow(gray_image)
plt.show()
plt.imshow(color_image)
plt.show()
plt.figure()
plt.title("Histogram")
plt.xlabel('Grayscale value')
plt.ylabel('pixel count')
plt.stem(hist)
plt.show()
plt.title('Histogram of color image - Green channel')
plt.xlabel('Intensity value')
plt.ylabel('pixel count')
plt.stem(hist1)
plt.show()






# Write the code to perform histogram equalization of the image. 
import cv2
g=cv2.imread('4.jpeg',0)
cv2.imshow('gray',g)
equ = cv2.equalizeHist(g)
cv2.imshow('Equalized image',equ)
cv2.waitKey(0)
cv2.destroyAllWindows()






```
## Output:
### Input Grayscale Image and Color Image
<br>![output](./op1.png)
<br>
<br>
<br>

### Histogram of Grayscale Image and any channel of Color Image
<br>![output](./op2.png)
<br>
<br>

### Histogram Equalization of Grayscale Image
![output](./op3.jpg)<br>
![output](./op4.jpg)

## Result: 
Thus the histogram for finding the frequency of pixels in an image with pixel values ranging from 0 to 255 is obtained. Also,histogram equalization is done for the gray scale image using OpenCV.
