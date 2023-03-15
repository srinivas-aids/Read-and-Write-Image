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

NAME: U.SRINIVAS

REG NO: 212221230108

### Register Number: 
i) #To Read,display the image
```
  import cv2
from google.colab.patches import cv2_imshow
a = cv2.imread('img.1.jpg',1)
cv2_imshow(a)
cv2.waitKey(0)

```
ii) #To write the image
```
colorImage = cv2.imread('img.1.jpg',1)
cv2.imwrite('img.1.jpg',colorImage)
writtenImage = cv2.imread('img.1.jpg',1)
cv2_imshow(writtenImage)
cv2.waitKey(0)


```
iii) #Find the shape of the Image
```python3
colorImage = cv2.imread('img.1.jpg',1)
print(colorImage.shape)


```
iv) #To access rows and columns

```python3
import random
colorImage = cv2.imread('img.1.jpg',1)
for i in range(100):
    for j in range(colorImage.shape[1]):
        colorImage[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2_imshow(colorImage)
cv2.waitKey(0)


```
v) #To cut and paste portion of image
```python3

color_img = cv2.imread('img.1.jpg',1)
tag = color_img[200:400,300:500]
color_img[200:400,100:300] = tag
cv2_imshow(color_img)
cv2.waitKey(0)

```

## Output:

### i) Read and display the image

![image](https://user-images.githubusercontent.com/93427183/225313357-ff1a9479-b828-42db-ab6c-f6fd061f5914.png)


### ii)Write the image

![image](https://user-images.githubusercontent.com/93427183/225313403-3cd141cf-4074-4bad-9672-be5a77de52d7.png)


### iii)Shape of the Image

<img width="258" alt="image" src="https://user-images.githubusercontent.com/93427183/225313564-38baaccd-1588-4939-99e7-2af144aa7587.png">

### iv)Access rows and columns
![image](https://user-images.githubusercontent.com/93427183/225313592-0c621c74-74e3-459e-bb37-2ace9478661e.png)


### v)Cut and paste portion of image
![image](https://user-images.githubusercontent.com/93427183/225313850-b4eecbea-3800-4ebb-95a0-b5ef7ec29a8b.png)


## Result:
Thus the images are read, displayed, and written successfully using the python program.


