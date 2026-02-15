# Fake News Detection System
Project Overview

The Fake News Detection System is a Machine Learning project developed using TensorFlow in Python. The main objective of this project is to classify news articles as Real or Fake based on their textual content.

The system uses Natural Language Processing techniques to preprocess text data and a deep learning model to perform classification.

Features

Text preprocessing and cleaning

Tokenization and sequence padding

Pre-trained word embeddings integration

Deep Learning model built using TensorFlow

Binary classification: Real or Fake

Model evaluation with accuracy and loss metrics

Technologies Used

Python

TensorFlow

NumPy

Pandas

Scikit-learn

Matplotlib

Project Structure
Fake-News-Detection/
│
├── dataset/
│   └── news_dataset.csv
│
├── glove.6B.50d.txt
│
├── app.py (if web application is included)
├── model_training.ipynb
├── requirements.txt
└── README.md

Dataset

The dataset contains news articles labeled as:

0 → Fake News

1 → Real News

The dataset is divided into training and testing sets for model development and evaluation.

Model Architecture

The model is built using TensorFlow Sequential API. The architecture includes:

Embedding Layer (with pre-trained GloVe embeddings)

Dropout Layer

Convolutional Layer (Conv1D)

MaxPooling Layer

LSTM Layer

Dense Output Layer with Sigmoid Activation

The model uses Binary Crossentropy as the loss function and Adam optimizer for training.

Installation

Clone the repository:

git clone <repository-link>
cd Fake-News-Detection


Install the required libraries:

pip install -r requirements.txt

How to Run

Open the Jupyter Notebook:

jupyter notebook model_training.ipynb


Run all cells to train the model.

If a web application is included:

python app.py

Model Training

Text data is cleaned and tokenized.

Sequences are padded to a fixed maximum length.

Word embeddings are loaded from GloVe.

The model is trained on the training dataset.

Performance is evaluated using test data.

Evaluation Metrics

Accuracy

Loss

Confusion Matrix

Future Improvements

Use larger and more diverse datasets

Improve preprocessing techniques

Experiment with different deep learning architectures

Deploy the model using cloud platforms

Author

Developed as a Machine Learning project using TensorFlow and Python.