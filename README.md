# LeNet-5 Implementation

A PyTorch implementation of the classic **LeNet-5 Convolutional Neural Network (CNN)** architecture proposed by Yann LeCun for handwritten digit recognition. This project demonstrates the fundamentals of convolutional neural networks through the implementation, training, and evaluation of LeNet-5 on the MNIST dataset.

## Overview

LeNet-5 is one of the earliest and most influential CNN architectures. Developed by Yann LeCun and his collaborators in 1998, it was designed for handwritten digit recognition and laid the foundation for modern deep learning in computer vision. :contentReference[oaicite:0]{index=0}

This project implements LeNet-5 from scratch using PyTorch to understand the core concepts behind convolutional neural networks.

---

## Features

- LeNet-5 architecture implemented from scratch
- MNIST handwritten digit classification
- Training and evaluation pipeline
- Accuracy and loss tracking
- GPU support through PyTorch
- Model checkpoint saving
- Visualization of training performance

---

## Architecture

The original LeNet-5 architecture consists of:

```text
Input Image (32×32)
        ↓
C1: Convolution Layer (6 feature maps)
        ↓
S2: Average Pooling
        ↓
C3: Convolution Layer (16 feature maps)
        ↓
S4: Average Pooling
        ↓
C5: Convolution Layer (120 feature maps)
        ↓
F6: Fully Connected Layer (84 neurons)
        ↓
Output Layer (10 classes)
```

LeNet-5 introduced key CNN concepts such as convolution, pooling, hierarchical feature extraction, and end-to-end learning. :contentReference[oaicite:1]{index=1}

---

## Dataset

### MNIST Dataset

The model is trained on the MNIST handwritten digit dataset:

- 70,000 grayscale images
- Image size: 28 × 28 pixels
- 10 digit classes (0–9)
- 60,000 training images
- 10,000 testing images

---

## Project Structure

```text
LeNET5-Implementation/
│
├── data/                   # Dataset files
├── models/                 # LeNet-5 architecture
├── outputs/                # Predictions and visualizations
├── checkpoints/            # Saved model weights
├── train.py                # Training script
├── test.py                 # Evaluation script
├── predict.py              # Inference script
├── requirements.txt
└── README.md
```

---

## Installation

Clone the repository:

```bash
git clone https://github.com/Anj-7171/LeNET5-Implementation.git
cd LeNET5-Implementation
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## Training

To train the model:

```bash
python train.py
```

The training process includes:

- Forward propagation
- Loss computation
- Backpropagation
- Weight updates using an optimizer
- Validation after each epoch

---

## Testing

Evaluate the trained model:

```bash
python test.py
```

Metrics reported:

- Test Accuracy
- Loss
- Classification Performance

---

## Inference

Run predictions on a custom image:

```bash
python predict.py --image sample.png
```

Example output:

```text
Predicted Digit: 7
Confidence: 99.2%
```

---

## Results

Typical LeNet-5 implementations achieve around 98–99% accuracy on MNIST. :contentReference[oaicite:2]{index=2}

---

## Key Concepts Learned

This project demonstrates:

- Convolution Operations
- Feature Extraction
- Pooling Layers
- Activation Functions
- Fully Connected Networks
- Backpropagation
- Image Classification

---

## Applications

Although originally developed for digit recognition, CNN architectures inspired by LeNet-5 are widely used in:

- Handwritten Text Recognition
- OCR Systems
- Medical Image Classification
- Face Recognition
- Object Detection
- Autonomous Systems

---

## Future Improvements

- Implement Batch Normalization
- Add Data Augmentation
- Compare with AlexNet and ResNet
- Hyperparameter Tuning
- Deploy as a Web Application
- Experiment with Fashion-MNIST and CIFAR-10

---

## References

1. Yann LeCun, Léon Bottou, Yoshua Bengio, and Patrick Haffner, *Gradient-Based Learning Applied to Document Recognition*, 1998. :contentReference[oaicite:3]{index=3}

2. LeNet-5 Architecture Documentation and PyTorch Implementations. :contentReference[oaicite:4]{index=4}

---

## Author

**Anjana Nair**

GitHub: https://github.com/Anj-7171

---

## License

This project is intended for educational and research purposes.
