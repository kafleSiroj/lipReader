# LipReader

LipReader is a deep learning application that interprets lip movements from video data and converts them into text. The model uses 3D Convolutional Neural Networks (3D-CNN) and Bidirectional LSTMs (BiLSTMs), trained on the GRID dataset with Connectionist Temporal Classification (CTC) loss for sequence alignment.

## Table of Contents

- [About the Project](#about-the-project)
- [Model Architecture](#model-architecture)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)

## About the Project

LipReader processes video clips to recognize spoken words by analyzing lip movements. This project is designed for offline processing and trained on a small subset of the GRID dataset. It incorporates ReLU activations, CTC loss, and is capable of handling varying-length sequences.

## Model Architecture

The architecture comprises:

1. **3D Convolutional Layers**: Extract spatiotemporal features from video frames.
2. **Bidirectional LSTMs (BiLSTM)**: Model temporal dependencies in the feature space.
3. **Dense Layer**: Maps LSTM outputs to character probabilities.
4. **CTC Loss**: Aligns input features to output sequences.

## Getting Started

### Prerequisites

- Python 3.8 or higher
- pip (Python package installer)
- GPU setup recommended for training.

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/kafleSiroj/lipReader.git
   cd lipReader
2. Install dependencies:
   ```bash
   pip install -r requirements.txt

