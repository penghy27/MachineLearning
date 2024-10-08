# README.md
## Project Overview:

This project utilizes a dataset provided by Zeta Surgical, consisting of brain CT scan slices with labeled hemorrhages. Hemorrhages are categorized into various types, including intraparenchymal, intraventricular, subarachnoid, subdural, epidural, and a category for images with normal brain type. The objective is to employ machine learning, computer vision, and data analytics to do the classification, regression and the segmentation of these CT images. The ultimate goal is to predict hemorrhage types and locations.

## Project Workflow:

**1. Image Preprocessing:**
Merge four windows of CT scan images: Each hemorrhage type has four subdirectories (brain_bone_window, brain_window, max_contrast_window, subdural_window) representing different rendering types. CT windowing facilitates rendering using various density values, with specific methods enhancing hemorrhage visibility. The raw dicom files have been converted to jpg format by the company. The 'normal/' folder contains images without hemorrhaging.

**2. Data Cleaning:**
Ensure original images have corresponding mask coordinates information. Convert these coordinates into mask images to maintain data integrity.

**3. Segmentation:**
Generate a predicted mask image to identify the hemorrhage area in the CT scans.

**4. Classification:**
Employ traditional machine learning and CNNs for predicting hemorrhage types.
