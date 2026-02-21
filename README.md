# Medical-Image-Segmentation-Study  
Study on Medical Segmentation  

This repository contains a series of experimental projects exploring different medical image segmentation techniques.

---

## 📂 Project 1: Brain MRI Tumor Segmentation (Otsu vs Sauvola)

### Objective:
Segment tumor regions in brain MRI slices using classical thresholding methods.

### Methods:
- Otsu (Global Thresholding)  
- Sauvola (Adaptive Thresholding)

### Evaluation Metrics:
- Dice Score  
- Jaccard Index  

### Dataset
https://www.kaggle.com/datasets/nikhilroxtomar/brain-tumor-segmentation

### Kaggle Notebook:
https://www.kaggle.com/code/naumisharanyatirth/brain-mri-tumor-segmentation  

### Key Finding: 
Both global and adaptive thresholding perform poorly for MRI tumor segmentation due to intensity overlap between tumor and normal brain tissues.

---
## 📂 Project 2: White Blood Cell Nucleus Segmentation (K-Means vs Fuzzy C-Means)

### Objective
Segment the nucleus region of White Blood Cells (WBC) using clustering-based methods.

### Methods
- K-Means (Hard Clustering)  
- Fuzzy C-Means (Soft Clustering)

### Evaluation
- Nucleus Area Comparison  
- Visual Boundary Comparison  

### Dataset
https://www.kaggle.com/datasets/paultimothymooney/blood-cells

### Kaggle Notebook
https://www.kaggle.com/code/naumisharanyatirth/white-blood-cell-segmentation-ipynb/edit

### Key Finding
Both methods segment the nucleus successfully. Fuzzy C-Means produces smoother boundaries due to soft clustering, while K-Means is faster but more rigid at edges.

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
https://www.kaggle.com/datasets/andrewmvd/drive-digital-retinal-images-for-vessel-extraction

### Kaggle Notebook
https://www.kaggle.com/code/naumisharanyatirth/retinal-vessel-extraction-sauvola-vs-niblack

### Key Finding
Niblack achieves high Sensitivity but tends to over-segment (low Dice due to noise).  
Sauvola provides cleaner segmentation with better Dice but moderate Sensitivity.  
Proper preprocessing and parameter tuning are necessary for accurate thin vessel extraction.

---
## 📂 Project 4: Cell Nuclei Separation (Watershed With vs Without Markers)

### Objective
Separate touching cell nuclei using watershed segmentation and compare performance with and without marker control.

### Methods
- Simple Thresholding (Without Markers)
- Marker-Controlled Watershed

### Evaluation Metric
- Dice Score

### Dataset
https://www.kaggle.com/c/data-science-bowl-2018

### Kaggle Notebook
https://www.kaggle.com/code/naumisharanyatirth/cell-nuclei-separation-ipynb/

### Key Finding
Simple thresholding achieved higher average Dice (0.7293) because many images had well-separated nuclei.
Marker-controlled watershed (0.6673) was useful in cases with overlapping nuclei by reducing over-segmentation.
Performance depends on image complexity.
 
