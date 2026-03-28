# The Math Behind The Aesthetic 💻✨

Ever wondered how Instagram filters actually work? Spoiler: It's just matrix algebra.

This repository contains the MATLAB script featured in my Reel breaking down Digital Image Processing (DIP). It proves that for a computer, a photo doesn't exist—it's just a 2D matrix of numbers from 0 to 255. Applying a "filter" is simply executing basic math operations on those numbers.

## What This Script Does

The code walks through three distinct mathematical operations on an image:

1. **The Moody Filter (Brightness Drop):** `I_new = I - 50` 
   Subtracts a constant value from every pixel to instantly drop the exposure.
2. **The Drama Filter (Extreme Contrast):** `I_new = 1.5 * I` 
   Multiplies the matrix by a scalar value, pushing the brights higher and the darks lower.
3. **The SVD Glitch Effect (Beat Drop):** Uses Singular Value Decomposition (SVD) to mathematically break down the RGB color channels. By reconstructing the image using fewer data points (dropping from 500 down to 5), it progressively destroys the image into a deep-fried, aesthetic blocky blur.

## How to Run It Locally

1. Clone or download this repository to your machine.
2. Place any image in the same folder as the script and rename it to `akii.jpg` (or just update line 5 of the code to match your image's filename).
3. Open the script in MATLAB.
4. Hit **Run**. 

The script will automatically generate a sleek, black-themed figure window and cycle through the transformations, pausing for a few seconds on each effect so you can see the math in real-time.

---
**Created by:** [@aayushayo](https://instagram.com/aayushayo)
