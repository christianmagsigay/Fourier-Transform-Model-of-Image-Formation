# Synthetic Images and Their Diffraction Patterns

---

## Overview

This Jupyter Notebook demonstrates the application of the **Discrete Fourier Transform (DFT)** in digital image processing to simulate physical optics phenomena and perform image analysis. The module focuses on simulating **Fraunhofer diffraction patterns** using synthetic apertures and applying **Fourier-based techniques** for convolution and pattern recognition.

---

## Objectives

The primary goals of this module are to:

- **Simulate Diffraction**  
  Perform the Discrete Fourier Transform (DFT) on synthetic images representing various apertures (e.g., circular apertures, double slits, gratings) to generate their corresponding Fraunhofer diffraction patterns.

- **Apply Convolution**  
  Perform convolution operations via the Fourier Transform using synthetic aperture images with varying diameters.

- **Template Matching**  
  Use correlation techniques to match a specific template with a target image (e.g., locating a letter or phrase within an image).

---

## Key Concepts

- **Discrete Fourier Transform (DFT)**  
  Converts spatial-domain images into the frequency domain, enabling simulation of far-field diffraction patterns.

- **Fraunhofer Diffraction**  
  A wave optics phenomenon observed in the far field when light passes through an aperture, simulated here using FFT-based methods.

- **Convolution Theorem**  
  Demonstrates that convolution in the spatial domain is equivalent to multiplication in the frequency domain.

- **Cross-Correlation**  
  A technique for template matching used to identify the position of a known pattern within a larger image.

---

## Dependencies

This notebook requires a Python environment with the following libraries:

- `numpy` — numerical operations and Fast Fourier Transforms  
- `matplotlib` — image display and plotting  
- `scikit-image (skimage)` — image input and processing (e.g., `skimage.io`, `skimage.color`)

---

## Usage

- **Synthetic Aperture Generation**  
  The notebook includes code to generate binary images representing various optical apertures, such as:
  - Circular apertures  
  - Annular apertures  
  - Double slits  
  - Diffraction gratings  

- **FFT Simulation**  
  Applies `np.fft.fft2` and `np.fft.fftshift` to aperture images to visualize their corresponding diffraction patterns.

- **Template Matching**  
  Loads a target image (e.g., text or symbols) and a template image, then applies Fourier-based correlation to localize the template within the target.

---

## Visual Outputs

The notebook produces several informative visualizations, including:

- Side-by-side plots of the **Aperture (Spatial Domain)** and its **Fast Fourier Transform (Frequency Domain)**  
- Visualizations illustrating **convolution effects**  
- **Template Matching** results showing correlation peaks where the template matches the target image  
