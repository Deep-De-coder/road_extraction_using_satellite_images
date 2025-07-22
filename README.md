# Road Extraction Using Satellite Images

![Project Banner](images/banner.png)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Last Update](https://img.shields.io/badge/last%20update-2024--06--09-blue)]()

---

## Table of Contents
- [Overview](#overview)
- [Project Structure](#project-structure)
- [Workflow](#workflow)
- [Features](#features)
- [Setup & Installation](#setup--installation)
- [Usage](#usage)
- [Results](#results)
- [Dataset](#dataset)
- [Reports & Video](#reports--video)
- [Authors](#authors)
- [References](#references)

---

## Overview
This project automates the extraction of road networks from satellite images using advanced deep learning techniques. It is designed for applications in urban planning, navigation, and disaster response. The solution leverages U-Net, model fusion, and various data augmentation and enhancement strategies to achieve robust segmentation results.

---

## Project Structure

```
.
├── Code/                        # Jupyter notebooks for all model stages
│   ├── Augmentation_models_code.ipynb
│   ├── Enhancement_Models.ipynb
│   └── Segmentation_models.ipynb
├── U_net.ipynb                  # U-Net model notebook
├── Model_Fusion.ipynb           # Model fusion notebook
├── images/                      # Place your result images here for README
├── Report/
│   └── 50544983_50538617_final_report.pdf
├── Video/
│   └── video.mp4
├── ProgressReport #2.pdf
├── computer_vision_project.zip  # Zipped code/data
├── 50544983_50538617_final_project.zip # Zipped full project
├── README.md
└── readme.txt                   # (Legacy)
```

---

## Workflow

```mermaid
graph TD;
    A[Satellite Images] --> B[Preprocessing & Augmentation];
    B --> C[Model Training (U-Net, Fusion)];
    C --> D[Prediction];
    D --> E[Post-processing];
    E --> F[Road Network Output];
```

---

## Features
- Deep learning-based segmentation (U-Net, model fusion)
- Data augmentation and enhancement
- Modular Jupyter Notebooks for each stage
- Visualizations of predictions vs. ground truth
- Comprehensive reports and video demonstration

---

## Setup & Installation

1. **Clone the repository**
2. **Install dependencies** (TensorFlow, Keras, OpenCV, Jupyter, etc.):
   ```bash
   pip install tensorflow keras opencv-python jupyter
   ```
3. **Download the dataset** (see [Dataset](#dataset))
4. **(Optional) Use Google Colab**: Update file paths as needed for your environment.

---

## Usage

Open and run the notebooks in the `Code/` directory or the root:
- `Code/Augmentation_models_code.ipynb`
- `Code/Enhancement_Models.ipynb`
- `Code/Segmentation_models.ipynb`
- `U_net.ipynb`
- `Model_Fusion.ipynb`

Example (in Jupyter):
```python
# In a notebook cell
!jupyter notebook Code/Segmentation_models.ipynb
```

---

## Results

Below are sample results. To add your own, place images in the `images/` folder and update the table:

| Input Image | Ground Truth | Predicted Mask |
|-------------|-------------|----------------|
| ![Input](images/input_example.png) | ![GT](images/ground_truth_example.png) | ![Pred](images/predicted_mask_example.png) |

---

## Dataset

- **Source**: [DeepGlobe Road Extraction Dataset](https://www.kaggle.com/datasets/balraj98/deepglobe-road-extraction-dataset)
- Download using Kaggle API or from the link above.
- For large files (e.g., pickles), see [Google Drive folder](https://drive.google.com/drive/folders/1VuYdE9l5sFM9tG18ZTDH_ruD0UeMbg3b?usp=sharing)
- Update file paths in notebooks as needed for your environment.

---

## Reports & Video

- **Final Report**: [`Report/50544983_50538617_final_report.pdf`](Report/50544983_50538617_final_report.pdf)
- **Progress Report**: [`ProgressReport #2.pdf`](ProgressReport%20#2.pdf)
- **Project Video**: [`Video/video.mp4`](Video/video.mp4)

---

## Authors

- *Your Name Here*
- *Collaborator Name (if any)*

---

## References

- [U-Net: Convolutional Networks for Biomedical Image Segmentation](https://arxiv.org/abs/1505.04597)
- [DeepGlobe Road Extraction Challenge](https://deepglobe.org/challenge.html)
- Any other relevant papers or resources

---

*For best results, add your own project images to the `images/` folder and update the image links above. Replace all placeholders with your actual data and results for a polished presentation.* 