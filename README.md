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
## Program
### Developed By : DHANUMALYA D
### Register Number : 212222230030 
i) #To Read,display the image
```
import cv2
color_img=cv2.imread('pup.jpg',1)
cv2.imshow('212222230030_DHANUMALYA',color_img)
cv2.waitKey(0)  

```
ii) #To write the image
```
import cv2
color_img=cv2.imread('pup.jpg',1)
w=cv2.imwrite('1.png',color_img)
cv2.imshow('212222230030_DHANUMALYA',color_img)
cv2.waitKey(0) 

```
iii) #Find the shape of the Image
```
import cv2
import random
color_img=cv2.imread('pup.jpg',1)
print(color_img.shape)

```
iv) #To access rows and columns

```
import cv2
import random
color_img=cv2.imread('pup.jpg',1)
for i in range(100):
    for j in range(color_img.shape[1]):
        color_img[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('212222230030_DHANUMALYA',color_img)
cv2.waitKey(0)

```
v) #To cut and paste portion of image
```
import cv2
color_image=cv2.imread('pup.jpg',-1)
tag=color_image[300:400,300:400]
color_image[50:150,50:150]=tag
cv2.imshow('212222230030_DHANUMALYA',color_image)
cv2.waitKey(0)

```

## Output:

### i) Read and display the image

![Screenshot from 2023-08-17 20-52-40](https://github.com/Dhanudhanaraj/READ-AND-WRITE-IMAGE/assets/119218812/34bb22fc-0d74-4b7f-ab85-6f2febe1aa35)




### ii)Write the image
![Screenshot from 2023-08-17 21-12-56](https://github.com/Dhanudhanaraj/READ-AND-WRITE-IMAGE/assets/119218812/1ac27797-9da9-465b-8ce7-7cb0cdb99c9f)




### iii)Shape of the Image

![Screenshot from 2023-08-17 21-08-02](https://github.com/Dhanudhanaraj/READ-AND-WRITE-IMAGE/assets/119218812/a5c28592-fb49-48ad-9fcc-21621b9ddc94)


### iv)Access rows and columns
![Screenshot from 2023-08-17 20-55-12](https://github.com/Dhanudhanaraj/READ-AND-WRITE-IMAGE/assets/119218812/7b896850-4cc3-422a-90e8-4b47dc35a6ef)



### v)Cut and paste portion of image
![Screenshot from 2023-08-17 20-54-41](https://github.com/Dhanudhanaraj/READ-AND-WRITE-IMAGE/assets/119218812/3e676b9a-d158-4bc4-b690-c9d12d9dd30d)




## Result:

Thus the images are read, displayed, and written successfully using the python program.
