# Week 2 – Mid Evaluation Assignment (OpenCV Fundamentals)

## Theme
Understanding OpenCV pipelines, not just function calls

---

## Tools Allowed
- Python
- OpenCV (`cv2`)
- NumPy
- Matplotlib

**Submission Format:** Jupyter Notebook (`.ipynb`)

**Important Instruction:**  
Use `matplotlib.pyplot.imshow()` to display images.  
**Do not use `cv2.imshow()` anywhere in the notebook.**

---

## Part A – Core OpenCV Skills
*(Everyone must attempt)*

---

### Q1. Image I/O and Color Spaces

- Load any **color image** of your choice using OpenCV.
- Display the image using **Matplotlib** (not `cv2.imshow()`).
- Convert the image into:
  - Grayscale
  - HSV
- Display all three images **side by side**.

**Answer in 2–3 lines:**
- Why does OpenCV read images in **BGR** instead of **RGB**?

**Expected Learning:**
- Color channel awareness
- OpenCV vs Matplotlib mismatch
- Conceptual clarity, not syntax

---

### Q2. Histogram Analysis

- Convert your image to **grayscale**.
- Plot the **grayscale histogram** using OpenCV.
- Apply **Histogram Equalization**.
- Plot the histogram **before and after** equalization.
- Display both images **side by side**.

**Answer briefly:**
- What visible change do you observe after equalization?
- In what kind of images is histogram equalization **not useful**?

---

### Q3. Image Smoothing and Noise Reduction

- Add **artificial noise** to a grayscale image.
- Apply the following filters:
  - Average Blur
  - Gaussian Blur
  - Median Blur
- Display all results in **one figure**.

**Answer:**
- Which filter handled noise best?
- Which filter preserved edges better?

---

### Q4. Geometric Transformations

- Resize the image to **half** its original size.
- Rotate the image by **45° about its center**.
- Translate the image by **(x = 50, y = 30)** pixels.
- Display all outputs clearly.

**Answer:**
- Why do geometric transformations often introduce **black regions**?

---

## Part B – Thresholding & Segmentation

---

### Q5. Manual vs Automatic Thresholding

- Convert an image to **grayscale**.
- Apply:
  - Global thresholding (manual threshold value)
  - Adaptive thresholding
  - Otsu’s thresholding
- Display all outputs **side by side**.

**Answer:**
- Which method worked best and why?
- When would global thresholding fail badly?

---

### Q6. Thresholding as Segmentation

- Choose an image where **foreground and background are distinguishable**.
- Use thresholding to isolate the **main object**.
- Show:
  - Original image
  - Binary image
  - Masked output

**Explain in 3–4 lines** how thresholding acts as segmentation.

---

## Part C – Thinking & Reflection
*(This section decides who actually understood)*

---

### Q7. Conceptual Reflection

Answer the following:

- Why is smoothing often applied **before thresholding**?
- Why is **HSV** sometimes better than **RGB** for segmentation?
- Can histogram equalization **negatively affect thresholding**? Explain.
- Why does OpenCV prefer **built-in functions** over manual pixel loops?

---

## Bonus (Optional)

Do **any one** of the following:

- Implement a small OpenCV pipeline:  
  **Read image → Smooth → Threshold → Geometric transform → Display**

**OR**

- Apply the same thresholding technique on **two very different images** and analyze the results.

---

## Notes

- Focus on **understanding the pipeline**, not just function calls.
- Clear visual outputs and concise explanations are expected.
- Code readability and correct OpenCV usage will be considered.
