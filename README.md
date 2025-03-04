# Hyperspectral_ENVI_Processing

# Hyperspectral Processing with ENVI

This project focuses on exploring hyperspectral data processing techniques using the ENVI software. The dataset utilized in this project is sourced from the Hyperion satellite, covering the steel mill area in Kraków, Poland, and its surroundings. The primary goal was to gain proficiency in ENVI tools and workflows, with a special emphasis on leveraging its built-in spectral library for analysis and detection of surface features.

---

## Table of Contents
1. [Project Assumptions](#project-assumptions)
2. [Data Loading](#data-loading)
3. [Working with Data](#working-with-data)
4. [Recording Data as NTIF](#recording-data-as-ntif)
5. [Hyperion Data Preprocessing](#hyperion-data-preprocessing)
6. [Removal of Artifacts from Hyperspectral Data](#removal-of-artifacts-from-hyperspectral-data)
7. [Data Format Conversion: BSQ to BIL](#data-format-conversion-bsq-to-bil)
8. [Atmospheric Correction: FLAASH](#atmospheric-correction-flaash)
9. [Atmospheric Correction: QUAC](#atmospheric-correction-quac)
10. [Smiling Removal](#smiling-removal)
11. [Principal Component Analysis (PCA)](#principal-component-analysis-pca)
12. [Channel Selection Without Interference](#channel-selection-without-interference)
13. [Classification](#classification)
    - [Supervised Classification](#supervised-classification)
    - [Unsupervised Classification](#unsupervised-classification)
14. [Summary and Conclusions](#summary-and-conclusions)
15. [Environmental Indicators](#environmental-indicators)
    - [Vegetation Index Calculator](#vegetation-index-calculator)
    - [Enhanced Vegetation Index (EVI)](#enhanced-vegetation-index-evi)
    - [NDWI](#ndwi)
    - [Moisture Stress Index](#moisture-stress-index)
    - [Band Math](#band-math)
    - [Intensity](#intensity)
    - [Forest Health](#forest-health)
16. [Global Spatial Statistics](#global-spatial-statistics)
17. [Object Detection Using Spectral Curves](#object-detection-using-spectral-curves)
    - [Topaz](#topaz)
    - [Asbestos](#asbestos)
    - [Construction Concrete](#construction-concrete)
18. [Submission](#submission)

---

## Project Assumptions
The main objective of this project was to master the ENVI software and its hyperspectral data processing capabilities. The Hyperion satellite data, covering the Kraków steel mill and adjacent areas, served as the foundation for this study. The processing pipeline was designed to explore ENVI’s functionalities, with a focus on its spectral library, and to perform basic detection analysis to identify characteristic surface features within the analyzed region.

---

## Data Loading
The project began with importing hyperspectral data into ENVI, ensuring proper handling of the multi-band dataset from the Hyperion satellite.

![image](https://github.com/user-attachments/assets/465efc46-d18a-4b84-9a87-ca0a10a2c8e3)

---

## Working with Data
Initial exploration involved visualizing and examining the hyperspectral dataset to understand its structure and spectral properties.

![image](https://github.com/user-attachments/assets/8660f15a-1da1-4158-b2d6-cc5ede53855f)

---

## Recording Data as NTIF
Data was saved in the NTIF format to ensure compatibility and efficient storage during processing.

---

## Hyperion Data Preprocessing
Preprocessing steps were applied to prepare the Hyperion data for further analysis, including calibration and noise reduction.

---

## Removal of Artifacts from Hyperspectral Data
Techniques were implemented to eliminate artifacts, such as sensor noise and data inconsistencies, enhancing the quality of the dataset.

---

## Data Format Conversion: BSQ to BIL
The data was converted from Band Sequential (BSQ) to Band Interleaved by Line (BIL) format to optimize processing workflows in ENVI.

---

## Atmospheric Correction: FLAASH
The Fast Line-of-sight Atmospheric Analysis of Spectral Hypercubes (FLAASH) module was used to correct atmospheric effects, improving data accuracy.

![image](https://github.com/user-attachments/assets/9fc14e26-311a-486d-b8c7-7c52b0c98c86)

---

## Atmospheric Correction: QUAC
Quick Atmospheric Correction (QUAC) was applied as an alternative method to FLAASH, offering a faster yet effective correction approach.

---

## Smiling Removal
The "smiling effect" (spectral distortion at the edges of the sensor) was corrected to ensure uniform spectral responses across the dataset.

![image](https://github.com/user-attachments/assets/1195d486-1734-4741-ab1d-b1a3e9acd0b6)

---

## Principal Component Analysis (PCA)
PCA was performed to reduce dimensionality and highlight the most significant spectral features in the dataset.

![image](https://github.com/user-attachments/assets/3cfbc410-4848-446e-9ffd-8dbc8a8a09ee)

---

## Channel Selection Without Interference
Channels free of atmospheric interference and noise were identified and selected for subsequent analysis.

---

## Classification
### Supervised Classification
Supervised techniques were employed to classify the data based on predefined training samples, targeting specific land cover types.

![image](https://github.com/user-attachments/assets/ec690ee6-0c96-4693-977f-de5de9d07838)

### Unsupervised Classification
Unsupervised methods, such as clustering, were used to explore natural groupings within the data without prior labeling.

![image](https://github.com/user-attachments/assets/f749f386-758c-4c5c-a693-d3b5eab3b4d1)

---

## Summary and Conclusions
The project provided a comprehensive understanding of ENVI’s tools, including atmospheric correction, classification, and spectral analysis. While classification results were satisfactory, further refinement is needed for more precise object detection.

---

## Environmental Indicators
### Vegetation Index Calculator
Various vegetation indices were computed to assess environmental conditions in the study area.

### Enhanced Vegetation Index (EVI)
EVI was calculated to evaluate vegetation health with improved sensitivity in high-biomass regions.

### NDWI
The Normalized Difference Water Index (NDWI) was used to monitor water content in vegetation and surface water bodies.

### Moisture Stress Index
This index helped identify areas experiencing moisture stress based on spectral reflectance.

### Band Math
Custom band math operations were applied to derive additional insights from the hyperspectral data.

### Intensity
Intensity metrics were calculated to analyze surface reflectance properties.

### Forest Health
Spectral data was used to assess forest health within the study area.

---

## Global Spatial Statistics
Spatial statistical tools were applied to analyze patterns and distributions across the dataset.
![image](https://github.com/user-attachments/assets/0d02a7af-71aa-42dd-b275-4089f589db84)

---

## Object Detection Using Spectral Curves
Spectral curve matching was used to detect specific materials and objects, leveraging ENVI’s spectral library.

### Topaz
Topaz deposits were identified using their unique spectral signatures.

### Asbestos
Asbestos-containing materials were detected based on their characteristic reflectance patterns.

### Construction Concrete
Concrete structures were mapped using spectral curve analysis.

![image](https://github.com/user-attachments/assets/e408ebfe-9000-45e1-9474-5087aacef802)

---

## Submission
Through this project, I deepened my knowledge of hyperspectral data processing and ENVI software. Key operations included atmospheric correction (FLAASH and QUAC), data format conversion, and supervised/unsupervised classification. The results demonstrated the potential of hyperspectral analysis, though further work is required to enhance object detection accuracy.

---

## Technologies Used
- **ENVI**: Hyperspectral data processing and analysis
- **Hyperion Satellite Data**: Source dataset
- **Spectral Library**: Material identification and classification

---
