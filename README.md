# Medical-Image-Segmentation-Study  
Study on Medical Segmentation  

This repository contains a series of experimental projects exploring different medical image segmentation techniques.

---

## 📂 Project 1: Brain MRI Tumor Segmentation (Otsu vs Sauvola)

**Objective:**  
Segment tumor regions in brain MRI slices using classical thresholding methods.

**Methods:**
- Otsu (Global Thresholding)  
- Sauvola (Adaptive Thresholding)

**Evaluation Metrics:**
- Dice Score  
- Jaccard Index  

**Kaggle Notebook:**  
https://www.kaggle.com/code/naumisharanyatirth/brain-mri-tumor-segmentation  

**Key Finding:**  
Both global and adaptive thresholding perform poorly for MRI tumor segmentation due to intensity overlap between tumor and normal brain tissues.

---
## 📂 Project 3: Retinal Vessel Extraction (Niblack vs Sauvola)

### Objective
Extract thin retinal blood vessels from fundus images using classical adaptive thresholding methods.

### Methods
- Niblack (Local Adaptive Thresholding)
- Sauvola (Improved Adaptive Thresholding)

### Evaluation Metrics
- Sensitivity
- Dice Score

### Dataset
DRIVE – Digital Retinal Images for Vessel Extraction

### Kaggle Notebook
https://www.kaggle.com/code/naumisharanyatirth/retinal-vessel-extraction-sauvola-vs-niblack

### Key Finding
Niblack achieves high Sensitivity but tends to over-segment (low Dice due to noise).  
Sauvola provides cleaner segmentation with better Dice but moderate Sensitivity.  
Proper preprocessing and parameter tuning are necessary for accurate thin vessel extraction.

## 🔜 Upcoming Projects

- Project 2  
- Project 4  
