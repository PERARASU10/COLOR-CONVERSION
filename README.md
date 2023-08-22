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


```
# iv)Split and Merge RGB Image
```


```
# v) Split and merge HSV Image
```



```
## Output:
### i) BGR and RGB to HSV and GRAY

![image](https://github.com/PERARASU10/COLOR-CONVERSION/assets/118348589/798f0c72-6b16-47af-9f24-c8b0444f6b3a)


### ii) HSV to RGB and BGR

![image](https://github.com/PERARASU10/COLOR-CONVERSION/assets/118348589/1cce5f7a-3552-4812-860d-49f6f03eea8a)


### iii) RGB and BGR to YCrCb
<br>
<br>

### iv) Split and merge RGB Image
<br>
<br>

### v) Split and merge HSV Image
<br>
<br>


## Result:
Thus the color conversion was performed between RGB, HSV and YCbCr color models.
