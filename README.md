# READ AND WRITE AN IMAGE
## AIM
To write a python program using OpenCV to do the following image manipulations.
i) Read, display, and write an image.
ii) Access the rows and columns in an image.
iii) Cut and paste a small portion of the image.

## Software Required:
Anaconda - Python 3.7
## Algorithm:
### Step1:
Choose an image and save it as a filename.jpg
### Step2:
Use imread(filename, flags) to read the file.
### Step3:
Use imshow(window_name, image) to display the image.
### Step4:
Use imwrite(filename, image) to write the image.
### Step5:
End the program and close the output image windows.
## Program:
### Developed By:
### Register Number: 
i) #To Read,display the image
```
 import cv2
colorImage = cv2.imread('/Users/eswar1607/Desktop/flower.png',1)
cv2.imshow('212221240035-Read&Display',colorImage)
cv2.waitKey(0)

```
ii) #To write the image
```
import cv2
colorImage = cv2.imread('/Users/eswar1607/Desktop/flower.png',1)
cv2.imwrite('/Users/eswar1607/Desktop/written.jpg',colorImage)
writtenImage = cv2.imread('/Users/eswar1607/Desktop/written.jpg',1)
cv2.imshow('212221240035-WrittenImage',writtenImage)
cv2.waitKey(0)

```
iii) #Find the shape of the Image
``python3
import cv2
colorImage = cv2.imread('/Users/eswar1607/Desktop/flower.png',1)
print(colorImage.shape)

```
iv) #To access rows and columns
```python3
import cv2
import random
colorImage = cv2.imread('/Users/eswar1607/Desktop/flower.png',1)
for i in range(100):
    for j in range(colorImage.shape[1]):
        colorImage[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('212221240035-AccessingRowsAndColumns',colorImage)
cv2.waitKey(0)

```
v) #To cut and paste portion of image
```python3
import cv2
color_img = cv2.imread('/Users/eswar1607/Desktop/flower.png',1)
tag = color_img[50:250,100:300]
color_img[100:300,50:250] = tag
cv2.imshow('212221240035-CutAndPaste',color_img)
cv2.waitKey(0)

```

## Output:

### i) Read and display the image

<br>
<img width="535" alt="Screenshot 2022-03-31 at 10 33 43 PM" src="https://user-images.githubusercontent.com/94154679/161112621-1e6dbda5-891d-4d67-b33b-a0343a0f9d63.png">
<br>

### ii)Write the image

<br>
<img width="535" alt="Screenshot 2022-03-31 at 10 36 46 PM" src="https://user-images.githubusercontent.com/94154679/161112838-93b28d50-c47d-4724-b6f4-237e6a8d643e.png">
<br>

### iii)Shape of the Image

<br>
<img width="835" alt="Screenshot 2022-03-31 at 10 38 05 PM" src="https://user-images.githubusercontent.com/94154679/161113115-62d95a0b-55fd-4929-a3d4-5d1e7d53a2c6.png">
<br>

### iv)Access rows and columns
<br>
<img width="535" alt="Screenshot 2022-03-31 at 10 39 33 PM" src="https://user-images.githubusercontent.com/94154679/161117621-5699cace-bc92-4297-93b6-a11df1dbdedb.png">
<br>

### v)Cut and paste portion of image
<br>
<img width="535" alt="Screenshot 2022-03-31 at 10 42 12 PM" src="https://user-images.githubusercontent.com/94154679/161113284-00b10313-efbc-488f-80b6-49cf5f363fc2.png">
<br>

## Result:
Thus the images are read, displayed, and written successfully using the python program.
