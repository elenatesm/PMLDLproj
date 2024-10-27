# PMLMDLProject
# Emotion Recognition Project

This project milestone aims to build a machine learning model that predicts human emotions based on textual input using natural language processing (NLP) techniques. The model is trained to recognize several emotions from a dataset of labeled texts.
In future applications, we aim to expand the capabilities of our solution. For example, collecting audio and video emotions. Also, extracting information from the provided text, audio, or video to extract key elements of speech and information.

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Model Architecture](#model-architecture)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Project Overview
The Emotion Recognition project is built using a Random Forest model trained on text data to classify emotions. The main steps involved include:
1. Preprocessing textual data.
2. Feature extraction using TF-IDF vectorization.
3. Training a Random Forest classifier.
4. Evaluating model performance through various metrics.

This project was developed as part of a course on Practical Machine Learning and Deep Learning (PMLDL).

## Dataset
The dataset used for training the model consists of labeled textual inputs, where each text is associated with an emotion (e.g., joy, sadness, anger, etc.). The key columns in the dataset are:
- `Clean_Text`: Preprocessed textual data.
- `Emotion`: Target emotion label.

If you want to use the dataset, make sure to upload it to the project directory as `emotion_dataset.csv`.

## Model Architecture
The project employs the following steps:
- **Text Preprocessing**: Lowercasing, removing punctuation, and cleaning the text.
- **TF-IDF Vectorization**: The text is converted into numerical form using TF-IDF (Term Frequency-Inverse Document Frequency) vectorization.
- **Random Forest Classifier**: A Random Forest model with 1000 trees is trained on the vectorized text.

## Installation
### Prerequisites
- Python 3.x
- Git
- `pip` for managing Python packages

### Steps to Install:
1. Clone the repository:
    ```bash
    git clone 
    git@github.com:elenatesm/PMLDLproj.git
    cd PMLMDLProject
    ```

2. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```

3. Prepare the dataset:
    - Place the dataset in the project directory as `emotion_dataset.csv`.

## Usage
### Training the Model
To train the model, use the following command:
```bash
python train_model.py
