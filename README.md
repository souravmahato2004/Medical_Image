# High-Precision Image Segmentation using U-Net Architecture

This repository contains the end-to-end implementation of a deep learning-based image segmentation pipeline developed during my tenure as an **AI Engineer at YantraPragya Developers**. The project focuses on pixel-wise semantic segmentation using a custom-engineered U-Net model.

## 🚀 Project Overview

The core objective was to develop a robust architecture capable of high-precision segmentation on **512x512 RGB images**. By implementing a symmetric encoder-decoder CNN from scratch, the model effectively captures complex semantic features while maintaining spatial resolution through skip connections.

### Key Highlights
* **From-Scratch U-Net:** Implementation of a symmetric CNN architecture.
* **Skip Connections:** Integrated to bridge the gap between contracting and expansive paths, ensuring precise localization.
* **Optimized Bottleneck:** Custom bottleneck layer designed for dense feature extraction.
* **End-to-End Pipeline:** Full data workflow from preprocessing and augmentation to model validation and inference visualization.

## 🛠️ Technical Stack

* **Deep Learning:** Python, TensorFlow/Keras (or PyTorch)
* **Image Processing:** OpenCV, NumPy
* **Visualization:** Matplotlib
* **Environment:** Jupyter Notebooks / Python Scripts

## 🧠 Model Architecture

The architecture follows the U-Net paradigm, consisting of:
1.  **Contracting Path (Encoder):** Successive convolutional and pooling layers to capture hierarchical context.
2.  **Bottleneck:** The latent space where the most abstract semantic features are extracted.
3.  **Expansive Path (Decoder):** Transposed convolutions to upsample feature maps to the original image resolution.
4.  **Skip Connections:** Concatenation of encoder feature maps with decoder layers to recover fine-grained spatial details.

## 📂 Repository Structure

```Medical_image
├── masks/
│   ├── masked_images       # Training loops and hyperparameters
├── Images/
│   └── original_images     # Model validation and visualization
├── assignment/             # Sample segmentation masks and metrics
├── requirements.txt        # Dependency list
└── README.md
