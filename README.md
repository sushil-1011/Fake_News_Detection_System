# Fake News Detection System

## Project Overview

The Fake News Detection System is a Machine Learning project developed using TensorFlow in Python.

The objective of this project is to classify news articles as Real or Fake based on textual content using Natural Language Processing and Deep Learning techniques.

The system preprocesses text data, converts it into numerical format, and trains a deep learning model to perform binary classification.


## Features

- Text cleaning and preprocessing
- Tokenization and sequence padding
- Integration of pre-trained GloVe word embeddings
- Deep Learning model built using TensorFlow
- Binary classification: Real or Fake
- Model evaluation using accuracy and loss


## Technologies Used

- Python
- TensorFlow
- NumPy
- Pandas
- Scikit-learn
- Matplotlib


## Project Structure

Fake-News-Detection/
│
├── dataset/
│   └── news_dataset.csv
│
├── glove.6B.50d.txt
├── model_training.ipynb
├── app.py
├── requirements.txt
└── README.md


## Dataset

The dataset contains labeled news articles:

- 0 -> Fake News
- 1 -> Real News

The dataset is divided into training and testing sets for model development and evaluation.


## Model Architecture

The model is built using TensorFlow Sequential API and includes:

- Embedding Layer with pre-trained GloVe embeddings
- Dropout Layer
- Conv1D Layer
- MaxPooling1D Layer
- LSTM Layer
- Dense Output Layer with Sigmoid Activation

Loss Function: Binary Crossentropy  
Optimizer: Adam


## Installation

Clone the repository:

git clone <repository-link>
cd Fake-News-Detection

Install required dependencies:

pip install -r requirements.txt


## How to Run

Run using Jupyter Notebook:

jupyter notebook model_training.ipynb

If using the web application:

python app.py


## Model Training Process

1. Load and clean the dataset
2. Perform text preprocessing
3. Tokenize text and create sequences
4. Apply padding to maintain fixed length
5. Load GloVe embeddings
6. Build and compile the model
7. Train the model
8. Evaluate performance on test data


## Evaluation Metrics

- Accuracy
- Loss
- Confusion Matrix


## Future Improvements

- Use larger and more diverse datasets
- Improve preprocessing techniques
- Experiment with advanced architectures
- Deploy the model on cloud platforms


## Author

Developed as a Machine Learning project using TensorFlow and Python.
