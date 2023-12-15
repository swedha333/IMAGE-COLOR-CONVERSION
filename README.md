# IMAGE-COLOR-CONVERSION
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
Choose an image and save it as a filename.jpg
### Step2:
Use imread(filename, flags) to read the file.
### Step3:
Use imshow(window_name, image) to display the image.
### Step4:
Use imwrite(filename, image) to write the image.
### Step5:
End the program and close the output image windows.
### Step6:
use cv2.COLOR_BGR2RGB to convert BGR to RGB

### Step7:
use cv2.COLOR_BGR2HSV to convert BGR to HSV

### Step8:
use cv2.COLOR_RGB2HSV to convert RGB to HSV

### Step9:
use cv2.COLOR_BGR2GRAY to convert BGR to GRAY

### Step10:
use cv2.COLOR_RGB2GRAY to convert RGB to GRAY

### Step11:
Display the original BGR image

### Step12:
Display the HSV image (BGR and RGB converted)

### Step13:
Display the Grayscale image (BGR and RGB converted)


## Program:

### Developed By:

### Register Number: 

i) #To Read,display the image
```
import cv2
from google.colab.patches import cv2_imshow



```
ii) #To write the image
```


print(f"Original image saved to: {image path}")



# Save the saved image to a new file
new_output_path = "Image path"
cv2.imwrite(new_output_path, saved_image)
print(f"Saved image saved to: {new_output_path}")
```
iii) #Save the saved image to a new file
```python3



```
iv) #Accessing rows and Columns
```python3


# Assign random values to pixels in the first row and first column
image[0, :] = np.random.randint(0, 256, size=(columns, channels))  # Random values for the first row
image[:, 0] = np.random.randint(0, 256, size=(rows, channels))  # Random values for the first column
```
v) #Cut and paste the image
```python3


# Get the shape of the image (rows, columns, channels)
rows, columns, channels = image.shape
print(f"Image Shape: Rows={rows}, Columns={columns}, Channels={channels}")
```
vi) #Convert BGR and RGB to HSV and GRAY
```python3
# Convert BGR to RGB
image_rgb = cv2.cvtColor(image_bgr, cv2.COLOR_BGR2RGB)
# Display the original BGR image
print("Original Image")
cv2_imshow(image_bgr)


```
vii) #Convert HSV to RGB and BGR
```python3



```
viii) #Convert RGB and BGR to YCrCb
```python3

# Convert RGB to YCrCb
image_rgb = cv2.cvtColor(image_bgr, cv2.COLOR_BGR2RGB)  # Convert BGR to RGB
image_ycrcb_rgb = cv2.cvtColor(image_rgb, cv2.COLOR_RGB2YCrCb)
# Display the YCrCb image (RGB to YCrCb)
print("RGB TO YCRCB")
cv2_imshow(image_ycrcb_rgb)


```
ix) #Split and Merge RGB Image
```python3



```
x) #Split and merge HSV Image
```python3



```
```

## Output:

### i) Read and display the image

<br>
<br>

### ii)Write the image

<br>
<br>

### iii)Shape of the Image

<br>
<br>

### iv)Access rows and columns

<br>
<br>

### v)Cut and paste portion of image

<br>
<br>

### vi) BGR and RGB to HSV and GRAY

<br>
<br>

### vii) HSV to RGB and BGR

<br>
<br>

### viii) RGB and BGR to YCrCb

<br>
<br>

### ix) Split and merge RGB Image

<br>
<br>

### x) Split and merge HSV Image

<br>
<br>

## Result:
Thus the images are read, displayed ,written and the color conversion was performed between RGB, HSV and YCbCr color models using the python program.
