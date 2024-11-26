# Impact of Max-Pooling on CNN Performance

This project examines the role of max-pooling layers in Convolutional Neural Networks (CNNs) for image classification tasks. The study compares architectures with and without max-pooling to highlight their impact on generalization, spatial detail retention, and learning behaviour.

---

## Overview
- **With Max-Pooling**: Reduces spatial dimensions, enhances generalization, and mitigates overfitting.
- **Without Max-Pooling**: Retains spatial details, increases susceptibility to overfitting, and changes learning dynamics.
- **Metrics**: Training loss, validation accuracy, test accuracy.

---

## Key Results
| Learning Rate | **Training Loss** | **Validation Accuracy** | **Test Accuracy** |
|---------------|-------------------|-------------------------|-------------------|
| **With Max-Pooling**            |                           |                     |                   |
| 0.1           | 0.6411            | 0.8183                  | 0.7958            |
| 0.01          | 0.5321            | 0.8753                  | **0.8374**        |
| 0.001         | 0.9591            | 0.7770                  | 0.7940            |
| **Without Max-Pooling**         |                           |                     |                   |
| 0.1           | 0.6733            | 0.7901                  | 0.7977            |
| 0.01          | 0.6508            | 0.8547                  | 0.8147            |
| 0.001         | 1.0540            | 0.6877                  | 0.7089            |

- Best performance: **With max-pooling** at a learning rate of 0.01 (test accuracy 83.7%).

---

## Methodology
- **With Max-Pooling**:
  - Downsamples feature maps using `MaxPool2D`.
  - Improves generalization and reduces overfitting.
- **Without Max-Pooling**:
  - Retains higher resolution features.
  - Processes detailed spatial information but risks overfitting.
- **Trainable Parameters**: Identical for both configurations (224,892).

---

## Technologies
- **Language**: Python
- **Framework**: PyTorch
- **Tools**: Matplotlib, Argparse

---

## Usage
1. Clone the repository:
   ```bash
   git clone https://github.com/anibalpires4/Impact-of-Max-Pooling-on-CNN-Performance.git

