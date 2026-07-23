# Medical Imaging System Analysis

University project developed for the **Medical Imaging Systems** course at the **University of Thessaly**.

## Overview

This project focuses on the quantitative evaluation of medical imaging systems. It combines medical image analysis, X-ray attenuation simulation and image-quality assessment methods.

The project includes:

- Modulation Transfer Function (MTF) estimation
- Gamma camera field homogeneity analysis
- X-ray attenuation simulation
- Image quality assessment
- Comparison of CT and SPECT system specifications

## Project Images

### Quadrant Phantom

The quadrant phantom contains line patterns with different spatial frequencies and was used for the MTF analysis.

![Quadrant Phantom](phantom_C9FF1H.gif)

### Gamma Camera Homogeneity Image

This image was used to evaluate variations in gamma camera field response.

![Gamma Camera Homogeneity](homogeneity_image_C9FF1A.gif)

## Main Results

### Modulation Transfer Function

The MTF analysis was performed using the quadrant phantom and an extracted intensity profile.

The maximum and minimum intensity values were used to estimate the system's ability to preserve image contrast at the selected spatial frequency.

- Maximum intensity: **143**
- Minimum intensity: **35**
- Calculated MTF: **0.6067**

The result provides a quantitative indication of the imaging system's capability to represent fine spatial structures.

### Gamma Camera Field Homogeneity

Field homogeneity was evaluated using a local **13 × 13 pixel** analysis window.

For each position, the local mean intensity was calculated. The maximum and minimum values were then used to evaluate the variation in detector response.

- Maximum intensity: **200**
- Minimum intensity: **87**
- Calculated homogeneity ratio: **0.5650**

This analysis can help identify non-uniform detector response, calibration problems or other technical variations in the gamma camera.

### X-ray Attenuation Simulation

The project also includes an X-ray attenuation simulation based on the Beer–Lambert law:

\[
I = I_0 e^{-\mu d}
\]

where:

- \(I\) is the transmitted intensity
- \(I_0\) is the incident intensity
- \(\mu\) is the linear attenuation coefficient
- \(d\) is the material thickness

The simulation uses a three-dimensional phantom containing regions with different attenuation coefficients and evaluates the effect of photon intensity and noise on the resulting image.

## Technologies and Topics

- MATLAB
- Medical Image Processing
- X-ray Imaging
- Gamma Camera Imaging
- Modulation Transfer Function
- Field Homogeneity Analysis
- Image Quality Assessment
- Biomedical Imaging
- CT and SPECT systems

## Repository Contents

- `MTF_2024/` — MTF analysis and project report
- `radiography.html` — X-ray attenuation simulation and generated results
- `phantom_C9FF1H.gif` — quadrant phantom used for MTF analysis
- `homogeneity_image_C9FF1A.gif` — gamma camera image used for homogeneity analysis

## Academic Context

This project was completed as part of the B.Sc. programme in **Computer Science with Biomedical Applications** at the **University of Thessaly**.

## Author

**Konstantinos Tsoumeleas**
