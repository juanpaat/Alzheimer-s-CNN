# Alzheimer’s Disease Detection and Classification Using MRI Data

## Overview

This repository contains the code and resources for the project *Alzheimer’s Disease Detection and Classification Using MRI Data*. The project employs Convolutional Neural Networks (CNNs) to classify Alzheimer's disease severity using MRI brain scans, focusing on early detection and accurate diagnosis. With Alzheimer's being a leading cause of death and a significant healthcare burden, this project aims to contribute to the development of efficient and cost-effective diagnostic tools using advanced machine learning techniques.

## Project Motivation

Alzheimer’s disease is a progressive neurodegenerative disorder that primarily affects older adults. Early detection is crucial for initiating timely treatment and improving the quality of life for those affected. However, traditional diagnostic methods can be time-consuming, expensive, and less accessible. This project explores the use of deep learning models for classifying Alzheimer's disease stages based on MRI images, providing a scalable solution to aid in the early detection and classification of the disease.

## Data

The dataset used in this project is the **Alzheimer_MRI Disease Classification Dataset** from [Hugging Face](https://huggingface.co/datasets/falah/Alzheimer_MRI_Disease_Classification). It contains MRI brain scans labelled into four categories:
- **0**: Mild Demented
- **1**: Moderate Demented
- **2**: Non Demented
- **3**: Very Mild Demented

### Dataset Information:
- **Training Data:**
  - Number of examples: 5,120
  - Size: ~22.6 MB
- **Test Data:**
  - Number of examples: 1,280
  - Size: ~5.6 MB

## Methodology

The project utilises CNN architectures to process and classify MRI images. CNNs are particularly effective in image recognition tasks, making them well-suited for identifying patterns in medical imaging data. The workflow involves:

1. **Data Preprocessing:** 
   - Loading MRI images, normalising, and resizing them for model compatibility.
   - Splitting the dataset into training and test sets.

2. **Model Development:**
   - Experimentation with different CNN architectures to identify the most suitable model for classifying Alzheimer's disease stages.
   - Fine-tuning the model based on performance metrics such as accuracy, precision, and recall.

3. **Model Evaluation:**
   - Evaluating the model’s performance using accuracy, confusion matrix, and classification reports.
   - Analysing the results to ensure that the model performs well in both multiclass and binary classification scenarios.

## Results

The final model achieved an overall classification accuracy of 96% for the four categories of Alzheimer’s severity. The binary classification model demonstrated high accuracy, precision, and recall, making it effective at identifying positive cases of dementia. These results show that CNNs can be a powerful tool for early detection and classification of Alzheimer’s disease, potentially assisting in faster and more accurate clinical diagnoses.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/alzheimer-disease-detection.git
   cd alzheimer-disease-detection
   ```
2. Install the required libraries:
   ```bash
   pip install -r requirements.txt
   ```

## Usage

1. **Data Preparation:**
   - Download the dataset from [Hugging Face](https://huggingface.co/datasets/falah/Alzheimer_MRI_Disease_Classification).
   - Place the dataset in the `data/` directory.

2. **Train the Model:**
   ```bash
   python train.py
   ```

3. **Evaluate the Model:**
   ```bash
   python evaluate.py
   ```

4. **View Results:**
   - Check the `results/` directory for performance metrics and visualisations.

## Contributing

Contributions are welcome! If you find any issues or want to suggest improvements, feel free to open a pull request or create an issue in the repository.


---

For more information, please refer to the [project report](./report.pdf).
