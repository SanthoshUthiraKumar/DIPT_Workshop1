# COLOR_CONVERSIONS_OF-IMAGE / Workshop1
## AIM
To write a python program using OpenCV to do the following image manipulations.

i) Read, display, and write an image.

ii) Access the rows and columns in an image.

iii) Convert image to gray scale and HSV 

iv)Display the H, S and V planes


## Software Required:
Anaconda - Python 3.7
## Algorithm:
### Step1: Choose an image and save it as a filename.jpg ,
### Step2: Use imread(filename, flags) to read the file.
### Step3: Use imshow(window_name, image) to display the image.
### Step4: Use imwrite(filename, image) to write the image.
### Step5: End the program and close the output image windows.
### Step6: Convert image to gray scale and HSV 
### Step7: Display the H, S and V planes

##### Program:
```
### Developed By: Santhosh U
### Register Number: 212222240092
```
<table>
  <tr>
    <td width=50%>

### i) 
```Python
import cv2
image=cv2.imread('flower.jpeg',1)
image=cv2.resize(image,(400,300))
cv2.imshow('Santhosh',image)
cv2.waitKey(0)
cv2.destroyAllWindows()
``` 
  </td>
  <td>

### OUTPUT:

 <img src="https://github.com/SanthoshUthiraKumar/DIPT_Workshop1/assets/119477975/1a1769fb-b180-4d5d-bf1c-0d5ac0b82017">
  </td>
  </tr>

   <tr>
    <td width=50%>


### ii)
```Python
import cv2
img = cv2.imread('flower.jpeg',1)
img = cv2.resize(img,(300,200))
cv2.imshow('Original Image',img)
hsv1 = cv2.cvtColor(img,cv2.COLOR_BGR2HSV)
cv2.imshow('OrginaltoHSV',hsv1)
gray1 = cv2.cvtColor(img,cv2.COLOR_BGR2GRAY)
cv2.imshow('OrginaltoGRAY',gray1)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
  </td>
  <td>

### OUTPUT:

<img src="https://github.com/SanthoshUthiraKumar/DIPT_Workshop1/assets/119477975/02fd6f7f-8ac1-4489-ab4e-6affcf354ef7">
  </td>
  </tr>
  <tr>
    <td width=50%>

### iii)
```Python
import cv2
img = cv2.imread("flower.jpeg",1)
img = cv2.resize(img,(300,200))
img=cv2.cvtColor(img,cv2.COLOR_RGB2HSV)
H,S,V=cv2.split(img)
cv2.imshow('Hue',H)
cv2.imshow('Saturation',S)
cv2.imshow('Value',V)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
  </td>
  <td>

### OUTPUT:

<img src="https://github.com/SanthoshUthiraKumar/DIPT_Workshop1/assets/119477975/715fe281-d723-43c7-b7cf-2b4d5d020429">
  </td>
  </tr>
  <tr>
    <td>


## Result:
Thus the images are read, displayed, and written ,and color conversion was performed between RGB, HSV and grayscale color models successfully using the python program.
