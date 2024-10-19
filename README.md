# Image Classification

![GitHub stars](https://img.shields.io/github/stars/potacon/image-classification?style=social)  
A deep learning project for image classification using a convolutional neural network (CNN). This repository provides a framework for training, testing, and deploying an image classifier using popular machine learning libraries.

#### If you use Google Colab, you can receive the files and run them sequentially.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Model Training](#model-training)
- [Testing the Model](#testing-the-model)
- [Configuration](#configuration)
- [Contributing](#contributing)
- [License](#license)

## Overview

This project is designed for image classification tasks, using a pre-trained CNN model or custom-built CNN architecture. It allows users to train models on custom datasets, fine-tune existing models, and deploy the trained classifier for inference.

## Features

- Supports custom datasets for training and testing
- Transfer learning using pre-trained models like ResNet, VGG, etc.
- Visualization of training metrics (loss, accuracy)
- Model evaluation and testing on test datasets
- Easy deployment of the trained model for inference

## Installation

### Prerequisites

- Python 3.8+
- Git

### Clone the Repository

```bash
git clone https://github.com/potacon/image-classification.git
cd image-classification
```

### Set Up a Virtual Environment
(Optional but recommended)

```bash
python3 -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`
```

### Install Dependencies
```bash
pip install -r requirements.txt
```

## Usage

### Model Training

1. Prepare your dataset and organize it into training and validation sets.
2. Update the configuration in the config.yaml file (if applicable) to set paths to your dataset and model parameters.
3. Run the training script:
```bash
python train.py --config config.yaml
```

### Testing the Model
To evaluate the model on a test set, run the following command:

```bash
python test.py --config config.yaml --weights path_to_trained_model.pth
```
### Inference
For running inference on new images using the trained model:
```bash
python infer.py --image path_to_image --weights path_to_trained_model.pth
```

### Configuration
You can modify various parameters in the config.yaml file, such as:

* Model architecture
* Dataset paths
* Learning rate
* Number of epochs
* Batch size
* Make sure to customize these parameters based on your dataset and computational resources..

## Contributing
Contributions are welcome! If you find bugs, want to add new features, or improve the documentation, feel free to submit a pull request. Make sure to follow the project's coding standards and document your changes.

### License
This project is licensed under the MIT License. See the LICENSE file for more details.

