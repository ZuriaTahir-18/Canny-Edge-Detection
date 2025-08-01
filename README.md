# Canny Edge Detection from Scratch in Python

This project is a step-by-step implementation of the **Canny Edge Detection** algorithm **from scratch**, written in Python using NumPy and OpenCV for image handling. The project is part of a computer vision assignment (CLO2 - C3) and focuses on building a strong understanding of edge detection techniques by manually implementing each phase of the algorithm.

---

## 📌 Objective

To implement the Canny edge detection pipeline from scratch, without relying on built-in OpenCV functions for edge detection. The project helps understand each phase of the process and visualizes its effect on the image.

---

## 🧠 Algorithm Steps Implemented

1. **Grayscale Conversion**  
   Convert the image to grayscale for simplification.

2. **Gaussian Blur**  
   Reduce image noise and smooth the image using a Gaussian filter.

3. **Sobel Filter (Gradient Calculation)**  
   Compute intensity gradients in the X and Y directions.

4. **Gradient Magnitude and Direction**  
   Combine X and Y gradients to get edge strength and angle.

5. **Non-Maximum Suppression**  
   Thin the edges by suppressing non-maximum pixels in the direction of the gradient.

6. **Double Thresholding**  
   Classify edges into strong, weak, and non-relevant based on high and low threshold values.

7. **Edge Tracking by Hysteresis**  
   Finalize the edges by linking weak edges to strong edges if they are connected.

---

## 🖼️ Example Output

| Original Image | Final Edge Detected Image |
|----------------|----------------------------|
| ![original](output/original.png) | ![canny](output/canny.png) |

> Note: Example images should be placed in an `output/` folder inside the repo.

---

## 📦 Requirements

- Python 3.x
- NumPy
- OpenCV (cv2)
- Matplotlib (for visualization)

Install dependencies using:

```bash
pip install numpy opencv-python matplotlib
