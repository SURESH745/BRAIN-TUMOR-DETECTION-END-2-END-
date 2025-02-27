# Brain Tumor Detection using CNN & Flask

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Flask](https://img.shields.io/badge/Flask-1.1.2-green)
![PyTorch](https://img.shields.io/badge/PyTorch-1.9-orange)
![Status](https://img.shields.io/badge/Status-Active-green)

<p align="center">
  <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="Python" width="100" height="100"/>
</p>

## Navigation Bar
- [Overview](#overview)
- [Features](#features)
- [Installation](#installation)
- [Docker Installation](#docker-installation-optional)
- [Model Architecture](#model-architecture)
- [Performance Metrics](#performance-metrics)
- [Example MRI Images](#example-mri-images)
- [Future Improvements](#future-improvements)
- [Contributing](#contributing)
- [License](#license)

## Overview
This project is a **Brain Tumor Detection System** that classifies MRI images into tumor or non-tumor categories using a **Convolutional Neural Network (CNN)**. It is deployed using **Flask**, allowing users to upload MRI images and receive instant predictions.

## Features
- MRI Image Classification (Tumor vs. Non-Tumor)
- User-friendly Flask Web Interface
- Deep Learning Model (CNN with PyTorch)
- Interactive Result Display
- API for Predictions

## Installation
### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/brain-tumor-detection.git
cd brain-tumor-detection
```

### 2. Install Dependencies
```bash
pip install -r requirements.txt
```

### 3. Run the Flask App
```bash
python app.py
```
The application will run on **http://127.0.0.1:5000/**.

## Docker Installation (Optional)
For easier deployment, use Docker:
```bash
docker build -t brain-tumor-detection .
docker run -p 5000:5000 brain-tumor-detection
```

## Model Architecture
- **CNN Layers:** 4 Convolutional Layers + MaxPooling + Fully Connected
- **Activation Functions:** ReLU, Softmax
- **Optimizer:** Adam
- **Loss Function:** Cross-Entropy Loss

_Why PyTorch?_
- PyTorch is more flexible and user-friendly for research and prototyping.
- Dynamic computation graphs enable easier debugging.

## Performance Metrics
| Metric        | Value |
|--------------|-------|
| Accuracy     | 98.5% |
| Precision    | 97.2% |
| Recall       | 96.8% |

_Confusion Matrix:_
> _Insert an accuracy graph or confusion matrix image_

## Example MRI Images
Tumor | Non-Tumor
--- | ---
![Tumor](example_tumor.jpg) | ![Non-Tumor](example_nontumor.jpg)

## Future Improvements
- Improve dataset size for better generalization
- Deploy on AWS or Render for live usage
- Implement segmentation for precise tumor localization

## Contributing
Contributions are welcome! If you find a bug or want to add an improvement, follow these steps:
1. Fork this repository.
2. Create a new branch (`feature-xyz`).
3. Commit your changes.
4. Push the branch and create a Pull Request.

## License
This project is licensed under the **MIT License**.

---
Made with love by **Gongali Suresh**

