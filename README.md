# Automatic CAPTCHA Recognition using CNN

## About the Project

This project is an AI-based CAPTCHA solver that automatically recognizes text-based CAPTCHAs using deep learning. It leverages a Convolutional Neural Network (CNN) to process CAPTCHA images and predict the characters with high accuracy.

## How It Works

### Dataset

The model is trained on the **CAPTCHA Version 2 dataset** from Kaggle.

Each CAPTCHA contains a combination of:

- Lowercase letters (`a-z`)
- Digits (`0-9`)

### Preprocessing

- Convert images to grayscale for better feature extraction.
- Resize images to a uniform **200 × 50 pixels**.
- Normalize pixel values to **[0, 1]** for efficient training.
- Convert text labels to one-hot encoded vectors.

## Model Architecture

The CNN model consists of:

- **Convolutional Layers (Conv2D)** for feature extraction.
- **MaxPooling Layers** to reduce spatial dimensions.
- **Batch Normalization** to improve convergence.
- **Fully Connected Layers (Dense Layers)** for classification.
- **Dropout Layers** to prevent overfitting.
- **Multiple output layers**, one for each character in the CAPTCHA.

## Training & Optimization

- **Loss Function:** Categorical Crossentropy
- **Optimizer:** Adam
- **Evaluation Metrics:** Accuracy, Validation Loss
- **Early Stopping:** Used to avoid overfitting.

## Evaluation & Results

- Accuracy and loss are tracked for both training and validation sets.
- The final model achieves high accuracy in recognizing CAPTCHA characters.

## Why This Project?

- **Security Research** – Understanding CAPTCHA vulnerabilities.
- **Machine Learning Practice** – Hands-on deep learning implementation.
- **Automation** – Eliminating manual CAPTCHA solving in repetitive tasks.

## Future Improvements

- Use Transfer Learning for improved accuracy on complex CAPTCHAs.
- Extend support for different CAPTCHA styles, such as distorted fonts , background noise and, lowercase + uppercase characters.
