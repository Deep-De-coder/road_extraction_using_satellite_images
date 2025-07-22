# Road Extraction Using Satellite Images

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
├── images/                      # (Optional) Place your result images here
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

### Pushing to GitHub: Personal Access Token Required

> **Note:** GitHub no longer supports password authentication for git operations over HTTPS. You must use a [Personal Access Token (PAT)](https://github.com/settings/tokens) instead of your GitHub password.

**How to push changes:**
1. Generate a token at [GitHub Tokens Settings](https://github.com/settings/tokens) (classic).
2. When prompted for a password during `git push`, paste your token instead of your GitHub password.
3. (Optional) Cache your credentials to avoid entering the token every time:
   ```sh
   git config --global credential.helper manager
   ```

For more details, see the [GitHub documentation](https://docs.github.com/en/github/authenticating-to-github/creating-a-personal-access-token).

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

Below are sample results. You can add your own results or visualizations by updating this section as needed.

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

- Deep Shahane

---

## References

- [U-Net: Convolutional Networks for Biomedical Image Segmentation](https://arxiv.org/abs/1505.04597)
- [DeepGlobe Road Extraction Challenge](https://deepglobe.org/challenge.html)
- Any other relevant papers or resources

--- 