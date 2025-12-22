# Assignment — Week 1: Image Basics (NumPy Only)

Goal  
The goal of this assignment is to understand how digital images are represented as matrices, how RGB color channels work, and how simple filters (convolution) affect images — using only NumPy and Matplotlib (no OpenCV).

Instructions  
- Use Python, NumPy, and Matplotlib only  
- Do not use OpenCV or any built-in image processing functions  
- Write clean, readable code  
- Add short explanations (1–2 lines) wherever appropriate  

Part A — Pixel and Color Basics  

Q1. Load and Display an Image  
Use matplotlib.image.imread() to load any image of your choice.  
Print the shape of the image.  
Print the minimum and maximum pixel values.  
Display the image using matplotlib.pyplot.imshow().

Q2. Separate and Combine Color Channels  
Extract the R, G, and B channels using NumPy slicing.  
Example:  
R = img[:, :, 0]  
G = img[:, :, 1]  
B = img[:, :, 2]  

Display each channel separately in grayscale.  
Combine the channels back using np.stack([R, G, B], axis=-1).  
Display the recombined image and verify it matches the original.

Q3. Convert RGB Image to Grayscale (Manually)  
Convert the image to grayscale using the formula:  
Gray = 0.299R + 0.587G + 0.114B  

Display the grayscale image.  
Compare it with np.mean(img, axis=2).  
Briefly comment on the visual difference.

Part B — Understanding Color Spaces  

Q4. Create an Artificial RGB Image  
Manually create a 3×3 RGB image using NumPy:  

img = np.array([  
  [[1,0,0],[0,1,0],[0,0,1]],  
  [[1,1,0],[0,1,1],[1,0,1]],  
  [[0.5,0.5,0.5],[1,1,1],[0,0,0]]  
])  

Print the RGB value of each pixel.  
For each pixel, describe the color you expect to see.

Q5. Simple RGB to Brightness Map  
Write a function:  

def brightness(img):  
    return np.max(img, axis=2)  

Apply it to the artificial image.  
Display the brightness map.  
Identify which areas appear bright and which appear dark.

Part C — Filters and Convolution  

Q6. 3×3 Blur Filter (Manual Convolution)  
Write a function:  

def blur_gray(img):  
    kernel = np.ones((3, 3)) / 9  
    # use manual convolution with loops  

Apply it to the grayscale image from Part A.  
Pad image borders with zeros using np.pad().  
Display the blurred image and compare it with the original grayscale image.

Part D — Reflection  

Answer briefly (2–3 lines each):  
What does a convolution kernel do?  
How does changing the kernel affect the output image?  
Why does grayscale conversion use weighted averages instead of a simple mean?

Submission  
Submit one Jupyter Notebook (.ipynb) containing code, outputs, and short explanations.  
You may use any image of size ≤ 512×512.  
Optional: include before/after comparison plots.

Important Note  
This assignment is intended for learning purposes.  
Students are strongly encouraged to attempt all questions independently before referring to any external resources.
