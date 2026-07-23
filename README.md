# Medical Imaging System Analysis

University project developed for the **Medical Imaging Systems** course at the **University of Thessaly**.

## Overview

This project focuses on the quantitative evaluation of medical imaging systems through image analysis and simulation techniques.

The work includes:

- Modulation Transfer Function (MTF) estimation
- Gamma camera field homogeneity analysis
- X-ray attenuation simulation
- Evaluation of image noise at different photon levels
- Comparison of CT and SPECT system specifications
- Medical imaging quality assessment

---

## X-ray Attenuation Simulation

The project includes the simulation of X-ray transmission through a three-dimensional phantom containing two spherical regions with different attenuation coefficients.

The transmitted intensity was calculated using the Beer–Lambert law:

\[
I = I_0 e^{-\mu d}
\]

where:

- \(I\) is the transmitted intensity
- \(I_0\) is the incident intensity
- \(\mu\) is the linear attenuation coefficient
- \(d\) is the material thickness

### X-ray Phantom Geometry

![X-ray Phantom Setup](Στιγμιότυπο%20οθόνης%202025-01-06%20213231.png)

The simulated phantom has dimensions of **256 × 256 × 128 mm** and contains:

- Sphere A with radius **25 mm**
- Sphere B with radius **12 mm**
- Different attenuation coefficients for the background and both spherical regions

### Simulation Output

The simulation evaluates image formation under different photon-count conditions, demonstrating the effect of noise on radiographic image quality.

The complete simulation and its generated results are available in:

- `radiography.html`
- `absorption_map.fig`
- `cases1,2_noise.fig`
- `intesity_case1,2.fig`
- `matlab.mat`

---

## Modulation Transfer Function Analysis

The Modulation Transfer Function was evaluated using a quadrant phantom containing parallel line patterns at different spatial frequencies.

### Quadrant Phantom

![Quadrant Phantom](phantom_C9FF1H.gif)

The analysis procedure included:

1. Selection of an image region containing a line pattern
2. Extraction of the intensity profile
3. Identification of the maximum and minimum intensity values
4. Calculation of the MTF value

The MTF was estimated using:

\[
MTF = \frac{P_{max}-P_{min}}{P_{max}+P_{min}}
\]

### Results

- Maximum intensity \(P_{max}\): **143**
- Minimum intensity \(P_{min}\): **35**
- Calculated MTF: **0.6067**

### MTF Intensity Profile

![MTF and Homogeneity Results](Στιγμιότυπο%20οθόνης%202025-01-20%20032042.png)

The calculated value provides a quantitative indication of the imaging system's ability to preserve contrast and represent fine spatial structures.

---

## Gamma Camera Field Homogeneity

Field homogeneity was evaluated using a gamma camera uniformity image.

### Input Image

![Gamma Camera Homogeneity Image](homogeneity_image_C9FF1A.gif)

The analysis was performed using a local **13 × 13 pixel** window.

For each image position, the local mean intensity was calculated. The maximum and minimum values were then identified and used to evaluate variations in detector response.

### Results

- Maximum intensity \(A_{max}\): **200**
- Minimum intensity \(A_{min}\): **87**
- Calculated homogeneity ratio: **0.5650**

The analysis also identifies the image locations at which the maximum and minimum local intensity values occur.

Field non-uniformity may indicate:

- Calibration errors
- Detector-response variations
- Technical problems affecting image quality
- Non-uniform gamma camera performance

---

## CT and SPECT System Comparison

The project also includes a comparison of technical specifications from selected CT and SPECT systems.

The comparison covers parameters such as:

- Number of slices
- Grayscale depth
- X-ray generator power
- Tube voltage
- Rotation period
- Spatial resolution
- MTF values
- Detector characteristics
- Energy resolution
- Sensitivity
- Maximum count rate

The specification comparison is available in:

- `Specifications.docx`

---

## Technologies and Topics

- MATLAB
- Medical image processing
- X-ray imaging
- Gamma camera imaging
- CT and SPECT systems
- Modulation Transfer Function
- Field homogeneity analysis
- Beer–Lambert law
- Image noise simulation
- Image quality assessment
- Biomedical imaging

---

## Repository Contents

- `MTF_2024/` — MTF analysis, exported results and project report
- `radiography.html` — X-ray attenuation simulation and generated output
- `phantom_C9FF1H.gif` — quadrant phantom used for MTF analysis
- `homogeneity_image_C9FF1A.gif` — gamma camera image used for homogeneity analysis
- `absorption_map.fig` — MATLAB attenuation-map figure
- `cases1,2_noise.fig` — simulated noisy-image results
- `intesity_case1,2.fig` — intensity results for the simulated cases
- `fig1.fig` and `fig2.fig` — additional MATLAB figures
- `matlab.mat` — MATLAB project data
- `Specifications.docx` — CT and SPECT specification comparison

---

## Key Learning Outcomes

Through this project, I gained practical experience in:

- Processing and evaluating medical images
- Performing quantitative image-quality measurements
- Calculating the Modulation Transfer Function
- Assessing gamma camera field homogeneity
- Simulating X-ray attenuation and image noise
- Interpreting technical specifications of medical imaging systems
- Using MATLAB for biomedical image analysis

---

## Academic Context

This project was completed as part of the B.Sc. programme in **Computer Science with Biomedical Applications** at the **University of Thessaly**.

---

## Author

**Konstantinos Tsoumeleas**
