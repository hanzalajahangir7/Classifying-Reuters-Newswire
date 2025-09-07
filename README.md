📰 Reuters Newswire Classification – Deep Learning with Keras

This project focuses on classifying Reuters news articles into 46 distinct topics using a deep learning model built with TensorFlow and Keras. The dataset is sourced from the built-in Reuters dataset available through Keras, containing thousands of short newswires labeled with topic categories.

📌 Objective

To build a multi-class text classification model that accurately predicts the topic of a news article based on its content. The model uses the 10,000 most frequently occurring words to represent the text data as binary vectors.

🧠 Model Overview

The model is a feedforward neural network with:

Input: One-hot encoded vectors of 10,000 dimensions

Hidden Layers: Two dense layers with 64 units and ReLU activation, each followed by dropout (0.5) and L2 regularization to reduce overfitting

Output Layer: A softmax layer with 46 units, one for each topic class

⚙️ Features

One-hot encoding for both input text and target labels

Dropout and L2 regularization for improved generalization

Model evaluation on a separate validation set

Training and validation metrics plotted using matplotlib

📊 Results

After training for 20 epochs, the model demonstrates strong classification performance on the test set, achieving high accuracy and generalizing well across various topics. Predictions are made by selecting the class with the highest softmax probability.

📉 Visualization

The project includes plots for:

Training vs. Validation Loss

Training vs. Validation Accuracy

These visualizations help identify overfitting and assess model learning over time.

🧪 Tools & Libraries

TensorFlow / Keras

NumPy

Matplotlib

🚀 Future Work

Replace one-hot encoding with word embeddings (e.g., Word2Vec or GloVe)

Experiment with LSTM or GRU for sequential learning

Optimize model with hyperparameter tuning

📁 Dataset

Reuters newswire dataset (from keras.datasets)

Limited to top 10,000 most frequent words
