# Impact of Max-Pooling on CNN Performance

This project explores the role of max-pooling layers in Convolutional Neural Networks (CNNs) for image classification tasks. The study highlights the trade-offs between retaining spatial detail and improving generalization by comparing architectures with and without max-pooling.

---

## Overview
The study involves:
- Implementing two CNN architectures:
  1. **With Max-Pooling**: Enhances generalization by reducing spatial dimensions.
  2. **Without Max-Pooling**: Retains spatial details by avoiding pooling layers.
- Evaluating performance across multiple learning rates.
- Analyzing accuracy, generalization, and trainable parameters for each configuration.

---

## Key Results
- **Best Validation Accuracy**: 87.5% (with max-pooling, learning rate = 0.01).
- **Best Test Accuracy**: 83.7% (with max-pooling).
- **Trainable Parameters**: 224,892 (identical across configurations).

---

## Technologies
- **Programming Language**: Python
- **Frameworks**: PyTorch
- **Tools**: Argparse, Matplotlib

---

## Usage
1. Clone the repository:
   ```bash
   git clone https://github.com/anibalpires4/Impact-of-Max-Pooling-on-CNN-Performance.git
