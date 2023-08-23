# COLOR-CONVERSION
## AIM
To perform the color conversion between RGB, BGR, HSV, and YCbCr color models.

## Software Required:
Anaconda - Python 3.7
## Algorithm:
### Step1:
Import cv2 library and upload the image or capture an image.
### Step2:
Read the saved image using cv2.imread("filename.jpg").

### Step3:
Convert the image into the given color transformation using cv2.cvtColor(image, cv2.BGR2YCrCb) and similarly for other color formats.
### Step4:
Split and merge the image using cv2.split(hsv) and cv2.merge([h,s,v]).
### Step5:
Output the image using cv2.imshow("OUTPUT", image).
## Program:
\
# Developed By: PERARASU M
# Register Number: 212222100033
# i) Convert BGR and RGB to HSV and GRAY
```
import cv2
houseImage = cv2.imread('benten.jpg')
cv2.imshow('212222100033_PERARASU',houseImage)
hsvImage = cv2.cvtColor(houseImage,cv2.COLOR_BGR2HSV)
cv2.imshow('BGR2HSV',hsvImage)
hsvImage1=cv2.cvtColor(houseImage,cv2.COLOR_RGB2HSV)
cv2.imshow('RGB2HSV',hsvImage1)
grayImage = cv2.cvtColor(houseImage,cv2.COLOR_BGR2GRAY)
cv2.imshow('BGR2GRAY',grayImage)
grayImage1 = cv2.cvtColor(houseImage,cv2.COLOR_RGB2GRAY)
cv2.imshow('RGB2GRAY',grayImage1)
cv2.waitKey(0)
cv2.destroyAllWindows()

```
# ii)Convert HSV to RGB and BGR
```
import cv2
houseHSVImage = cv2.imread('benten.jpeg')
cv2.imshow('212222100033_PERARASU',houseHSVImage)
RGBImage = cv2.cvtColor(houseHSVImage,cv2.COLOR_HSV2RGB)
cv2.imshow('BGR2HSV',RGBImage)
BGRImage=cv2.cvtColor(houseHSVImage,cv2.COLOR_HSV2BGR)
cv2.imshow('RGB2HSV',BGRImage)
cv2.waitKey(0)
cv2.destroyAllWindows()


```
# iii)Convert RGB and BGR to YCrCb
```
import cv2
houseImage = cv2.imread('benten.jpg')
cv2.imshow('212222100033_PERARASU',houseImage)
YCrCb_image = cv2.cvtColor(houseImage, cv2.COLOR_RGB2YCrCb)
cv2.imshow('BGR2HSV',YCrCb_image)
YCrCb_image1 = cv2.cvtColor(houseImage, cv2.COLOR_BGR2YCrCb)
cv2.imshow('RGB2HSV',YCrCb_image1)
cv2.waitKey(0)
cv2.destroyAllWindows()

```
# iv)Split and Merge RGB Image
```
import cv2
image = cv2.imread('benten.jpg')
blue = image[:,:,0]
green = image[:,:,1]
red = image[:,:,2]
cv2.imshow('B-Channel',blue)
cv2.imshow('G-Channel',green)
cv2.imshow('R-Channel',red)
mergeBgr = cv2.merge((blue,green,red))
cv2.imshow('212222100033_PERARASU',mergeBgr)
cv2.waitKey(0)
cv2.destroyAllWindows()

```
# v) Split and merge HSV Image
```
import cv2
image = cv2.imread('benten.jpg')
hsv = cv2.cvtColor(image,cv2.COLOR_BGR2HSV)
h,s,v = cv2.split(hsv)
cv2.imshow('Hue - Image',h)
cv2.imshow('Saturation - Image',s)
cv2.imshow('Gray - Image',v)
mergedHSV = cv2.merge((h,s,v))
cv2.imshow('212222100033_PERARASU',mergedHSV)
cv2.waitKey(0)
cv2.destroyAllWindow()


```
## Output:
### i) BGR and RGB to HSV and GRAY

![image](https://github.com/PERARASU10/COLOR-CONVERSION/assets/118348589/798f0c72-6b16-47af-9f24-c8b0444f6b3a)


### ii) HSV to RGB and BGR

![image](https://github.com/PERARASU10/COLOR-CONVERSION/assets/118348589/1cce5f7a-3552-4812-860d-49f6f03eea8a)


### iii) RGB and BGR to YCrCb

![image](https://github.com/PERARASU10/COLOR-CONVERSION/assets/118348589/f1812e9b-1e18-4937-b84f-f5c84168b69d)


### iv) Split and merge RGB Image

![image](https://github.com/PERARASU10/COLOR-CONVERSION/assets/118348589/822c3763-d452-4d82-ab86-fcedbfc04810)

### v) Split and merge HSV Image

![image](https://github.com/PERARASU10/COLOR-CONVERSION/assets/118348589/ed7511f0-10cf-47bb-8e85-888e5f8109bc)


## Result:
Thus the color conversion was performed between RGB, HSV and YCbCr color models.
