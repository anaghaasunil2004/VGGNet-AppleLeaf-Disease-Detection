# VGGNet-AppleLeaf-Disease-Detection

This repository contains a **VGG16** deep learning model for detecting apple leaf diseases. The model classifies leaves into **Healthy, Rust, Scab, or Multiple Diseases** using hierarchical feature extraction.

![image](https://github.com/user-attachments/assets/fc648d8a-9d7e-426c-8205-b70d4d737345)![image](https://github.com/user-attachments/assets/5c8525cb-057d-4a16-af33-b9becdda3045)![image](https://github.com/user-attachments/assets/7373b489-1ca5-434c-b42b-bafe6d691db1)![image](https://github.com/user-attachments/assets/2fa3d99d-28da-4e52-b16c-b0571ecd1bdb)

## Dataset
- Dataset:[Plant Pathology 2020 - FGVC7 | Kaggle](https://www.kaggle.com/competitions/plant-pathology-2020-fgvc7)
- Includes labeled apple leaf images.

## Model Overview
- **VGG16 architecture** with a simple 3×3 convolutional structure.
- Uses **pre-trained ImageNet weights** for transfer learning.
- Fully connected layers followed by a **Softmax classifier**.
- Struggles with high parameter count and computational cost.

## Installation & Requirements
To run this project, install dependencies:
```bash
pip install tensorflow keras numpy pandas matplotlib seaborn
```

## Usage
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/VGG16-AppleLeaf-Disease-Detection.git
   cd VGG16-AppleLeaf-Disease-Detection
   ```
2. Open and run `vgg16_model.ipynb` in Jupyter Notebook or Google Colab.
3. Load the dataset and train the model.

## Results
- Achieved **21% accuracy**, struggling with complex disease patterns.
- Underperforms due to its **high parameter count** and **lack of skip connections**.

## Future Improvements
- Using **data augmentation** to improve generalization.
- Exploring **depthwise separable convolutions** to reduce computational cost.

## License
This project is licensed under the **MIT License**.
