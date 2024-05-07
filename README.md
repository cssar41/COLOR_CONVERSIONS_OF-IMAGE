# COLOR_CONVERSIONS_OF-IMAGE
## AIM
To write a python program using OpenCV to do the following image manipulations.

i) Read, display, and write an image.

ii) Access the rows and columns in an image.

iii) Cut and paste a small portion of the image.

iv)To perform the color conversion between RGB, BGR, HSV, and YCbCr color models.


## Software Required:
Anaconda - Python 3.7
## Algorithm:
### Step1:
Choose an image and save it as a filename.jpg ,
### Step2:
Use imread(filename, flags) to read the file.
### Step3:
Use imshow(window_name, image) to display the image.
### Step4:
Use imwrite(filename, image) to write the image.
### Step5:
End the program and close the output image windows.
### Step6:
Convert BGR and RGB to HSV and GRAY
### Step7:
Convert HSV to RGB and BGR
### Step8:
Convert RGB and BGR to YCrCb
### Step9:
Split and Merge RGB Image
### Step10:
Split and merge HSV Image

## Program:
### Developed By: Saravanan C
### Register Number: 212222110041
i) #To Read,display the image
```python3
import cv2
img = cv2.imread('car.jpg', 0)
resized_img = cv2.resize(img, None, fx=0.1, fy=0.1)
cv2.imshow('212222110041', resized_img)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
ii) #To write the image
```python3
import cv2
img=cv2.imread('car.jpg',0)
cv2.imwrite('writed_walt.png',img)
```
iii) #Find the shape of the Image
```python3
import cv2
img=cv2.imread('car.jpg',0)
print(img.shape)
```
iv) #To access rows and columns
```python3
import cv2
img = cv2.imread('car.jpg', 0)
resized_img = cv2.resize(img, None, fx=0.1, fy=0.1)
for i in range(100, 250):
    for j in range(10, 50):
        resized_img[i][j] = 255  # Set the pixel to white
cv2.imshow('212222110041', resized_img)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
v) #To cut and paste portion of image
```python3
import cv2
img = cv2.imread('car.jpg', 0)
resized_img = cv2.resize(img, None, fx=0.1, fy=0.1)
copied_portion = resized_img[150:250, 250:450]
resized_img[10:110, 10:210] = copied_portion
cv2.imshow('212222110041', resized_img)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
## Output:

### i) Read and display the image
(![1 (2)](https://github.com/cssar41/COLOR_CONVERSIONS_OF-IMAGE/assets/159455133/c27ef15a-8bf5-4584-ac92-88955a72203f)
### ii)Write the image
![3](https://github.com/cssar41/COLOR_CONVERSIONS_OF-IMAGE/assets/159455133/17fb257f-fd12-434f-bac1-8e83df32ac13)
### iii)Shape of the Image
![4](https://github.com/cssar41/COLOR_CONVERSIONS_OF-IMAGE/assets/159455133/9aeac698-2e15-43bf-9c4d-e04ce2315a0c)
### iv)Access rows and columns
![5 (2)](https://github.com/cssar41/COLOR_CONVERSIONS_OF-IMAGE/assets/159455133/f0c391ca-b63e-4fff-9e09-b87a6e4d065e)
### v)Cut and paste portion of image
![6 (2)](https://github.com/cssar41/COLOR_CONVERSIONS_OF-IMAGE/assets/159455133/54fe06f8-67d5-4069-b791-be87a3218f01)



## Result:
Thus the images are read, displayed, and written ,and color conversion was performed between RGB, HSV and YCbCr color models successfully using the python program.







