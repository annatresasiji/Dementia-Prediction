# Dementia-Prediction
# Screening Tool for Dementia

A Multimodal Hybrid Deep Learning Framework for Early Dementia Detection using MRI and Cognitive Assessment.

## Overview

Dementia is a progressive neurodegenerative condition that affects memory, cognition, and daily functioning. Early detection is essential for timely clinical intervention and improved patient outcomes.

This project presents a hybrid deep learning framework that integrates cognitive assessment scores with MRI-based neuroimaging analysis for early dementia detection. By combining standardized cognitive screening measures with deep learning-derived imaging features, the framework aims to improve diagnostic accuracy and support clinical decision-making.

---

## Objectives

* Develop an automated system for dementia screening.
* Integrate cognitive assessment scores with MRI-derived features.
* Evaluate the effectiveness of multimodal learning for dementia detection.
* Compare the performance of multiple deep learning architectures.
* Improve early identification of Mild Cognitive Impairment (MCI) and dementia.

---

## Methodology

The proposed framework consists of the following stages:

1. Patient data collection
2. Cognitive assessment using:

   * Mini-Mental State Examination (MMSE)
   * Abbreviated Mental Test Score (AMTS)
3. MRI acquisition and preprocessing
4. Deep feature extraction using:

   * ResNet50
   * DenseNet121
5. Multimodal feature fusion
6. Classification using a fully connected neural network
7. Dementia prediction

---

## Dataset

The framework utilizes the Open Access Series of Imaging Studies (OASIS) dataset.

Dataset characteristics include:

* Structural MRI scans
* Clinical metadata
* Cognitive assessment information
* Longitudinal neuroimaging records

Dataset: https://www.oasis-brains.org/

---

## Models

### ResNet50

ResNet50 is employed for extracting high-level spatial representations from MRI scans through residual learning, enabling effective modeling of structural brain changes associated with dementia.

### DenseNet121

DenseNet121 utilizes dense connectivity to improve feature reuse and capture fine-grained neuroanatomical variations that may indicate cognitive decline.

---

## Performance

| Metric               | ResNet50 | DenseNet121 |
| -------------------- | -------- | ----------- |
| Test Accuracy        | 87.0%    | 84.0%       |
| Precision            | 0.78     | 0.79        |
| Recall (Sensitivity) | 71.1%    | 85.2%       |
| Specificity          | 86.2%    | 75.1%       |
| F1 Score             | 0.74     | 0.82        |

### Comparison with Baseline Approaches

| Method                    | Accuracy (%) |
| ------------------------- | ------------ |
| Logistic Regression       | 72.5         |
| Support Vector Machine    | 75.8         |
| CNN (MRI Only)            | 84.0         |
| Proposed Hybrid Framework | 87.0         |

---

## Technology Stack

### Programming Language

* Python

### Deep Learning Frameworks

* PyTorch
* TorchVision

### Data Processing and Analysis

* NumPy
* Pandas
* OpenCV
* Scikit-learn

### Visualization

* Matplotlib
* Grad-CAM

---

## Project Structure

```text
Screening_tool_for_dementia/
│
├── data/
├── preprocessing/
├── models/
├── training/
├── evaluation/
├── notebooks/
├── results/
├── app/
├── requirements.txt
└── README.md
```

---

## Installation

Clone the repository:

```bash
git clone https://github.com/your-username/Screening_tool_for_dementia.git
```

Navigate to the project directory:

```bash
cd Screening_tool_for_dementia
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## Usage

Train the model:

```bash
python train.py
```

Run inference:

```bash
python predict.py
```

---

## Future Work

* Multi-class dementia staging
* Integration of Vision Transformers
* Longitudinal disease progression modeling
* Inclusion of PET and fMRI modalities
* Explainable AI enhancements
* Clinical decision-support deployment
* Integration with electronic health records

---

## Authors

Anna Tresa Siji
Department of Computer Science and Engineering
Amrita Vishwa Vidyapeetham, Amritapuri

Kunche Revanth Satya Sai Raghuveer
Department of Computer Science and Engineering
Amrita Vishwa Vidyapeetham, Amritapuri

B. R. Govind
Department of Computer Science and Engineering
Amrita Vishwa Vidyapeetham, Amritapuri

### Supervisor

Ani R
Department of Computer Science and Engineering
Amrita Vishwa Vidyapeetham, Amritapuri

---

## Citation

If you use this work in your research, please cite the associated publication:

*Anna Tresa Siji, Kunche Revanth Satya Sai Raghuveer, B. R. Govind, and Ani R., "A Multimodal Hybrid Deep Learning Framework for Early Dementia Detection using MRI and Cognitive Assessment."*

---

## License

This project is intended for academic and research purposes.
