# Assignment 3 — Morphology, Edges, Frequency & Shape (Applied)

### Rule of Thumb
> **If you can’t show it visually, you don’t understand it yet.**

---

## 🛠 Tools Allowed
- Python  
- NumPy  
- OpenCV  
- Matplotlib  

---

## 📦 Submission Format
- **Single Jupyter Notebook (`.ipynb`)**
- Each task in a **separate section**
- **All outputs must be visible**
- Observations must be **short, practical, and honest**

---

## Task 1 — Binary Image + Structuring Element

### What to do
- Load any **grayscale image**
- Convert it to a **binary image** using thresholding
- Create **three different structuring elements**:
  - 3×3 square  
  - 3×3 cross  
  - 5×5 square  

### Output
Display:
- Binary image  
- Result of **dilation** using each structuring element (**side by side**)

### Constraint
- ❌ Do not reuse the same structuring element shape twice

### Observation *(1–2 lines in comments)*
- How does changing the **structuring element shape** affect object growth?

---

## Task 2 — Noise Removal Without Touching the Object

### What to do
- Add **salt noise** to the binary image
- Remove noise using **only morphological operations**

You may use:
- Erosion  
- Dilation  
- Opening  
- Closing  

### Output
Display:
- Noisy image  
- Cleaned image  

### Constraints
- ❌ No blurring  
- ❌ No median filter  

### Observation
- Which morphological operation was **most effective**, and why?

---

## Task 3 — Fill Gaps in Broken Objects

### What to do
- Take a **binary image** where objects have small holes or breaks
- Use morphology to:
  - Fill holes  
  - Preserve object size as much as possible  

### Output
Display:
- Before  
- After  

### Observation
- What happens if the **structuring element size is too large**?

---

## Task 4 — Sobel vs Canny (Edge Reality Check)

### What to do
- Convert a **natural image** to grayscale
- Apply:
  - Sobel edge detection  
  - Canny edge detection  

### Output
Display:
- Original image  
- Sobel result  
- Canny result  

### Constraint
- Use **at least two different Canny threshold pairs**

### Observation
- Which edges **disappear first** as thresholds increase?

---

## Task 5 — Line Detection from Scratch (Pipeline Thinking)

### What to do
- Use the **Canny output**
- Apply **Hough Line Transform**
- Draw detected lines on the **original image**

### Output
Display:
- Canny edges  
- Final image with detected lines  

### Constraint
- ❌ Do not tune blindly  
- Change **one parameter at a time**

### Observation
- What happens when the **Hough threshold is too low**?

---

## Task 6 — Fourier Transform: See the Invisible

### What to do
- Compute the **2D Fourier Transform** of a grayscale image
- Display the **magnitude spectrum**
- Apply:
  - Low-pass filtering  
  - High-pass filtering  
- Reconstruct images using **inverse FFT**

### Output
Display:
- Original image  
- Frequency spectrum  
- Low-pass filtered result  
- High-pass filtered result  

### Observation
- Which operation affects **edges** more?

---

## Task 7 — Contours as Object Boundaries

### What to do
- Threshold an image
- Detect contours
- Identify and draw:
  - All contours  
  - Largest contour only  

### Output
Display:
- Contours overlaid on the original image  

### Constraint
- ❌ Do not use edge detection before contour extraction

### Observation
- What happens if **thresholding is poor**?

---

## Final Challenge — Combine Everything

### What to do
Using **any image of your choice**:
- Use morphology to clean the image
- Detect edges
- Extract contours
- Highlight **only meaningful object boundaries**

### Output
- A **single final image** showing clean object outlines

---

## 🚨 Submission Rules (Strict)
- Only **one `.ipynb` file**
- Each task must have a **clearly marked section**
- All outputs must be **visible**
- Observations must be **brief and insightful**

---
