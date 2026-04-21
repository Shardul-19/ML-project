# ML-project
MNIST Handwritten Digit Recognition — CNN
A Convolutional Neural Network built with TensorFlow/Keras that classifies handwritten digits (0–9) from the MNIST dataset with ~99% test accuracy.

📌 Overview
This project implements a deep CNN trained on the classic MNIST dataset. It demonstrates the power of convolutional layers over simple Dense networks — achieving ~2% accuracy gain over a baseline Dense NN.
ModelTest AccuracyDense Neural Network97.2%CNN (this project)~99.0%

🏗️ Model Architecture
Input: (28, 28, 1)
│
├── Conv2D(32, 3×3, ReLU)
├── MaxPooling2D(2×2)
├── Conv2D(64, 3×3, ReLU)
├── MaxPooling2D(2×2)
├── Conv2D(64, 3×3, ReLU)
├── Flatten
├── Dense(64, ReLU)
├── Dropout(0.5)
└── Dense(10, Softmax)

Optimizer: Adam
Loss: Categorical Crossentropy
Epochs: 5
Batch Size: 128


📁 Project Structure
Mnist_CNN_99percent/
│
├── Mnist_CNN.ipynb       # Main notebook — training, evaluation, visualization
└── README.md

⚠️ The saved model file (mnist_cnn_99.h5) is auto-generated on run and is excluded from this repo.


🚀 How to Run
Option 1: Google Colab (Recommended)
Click the badge below to open directly in Colab:
Show Image
Option 2: Run Locally
1. Clone the repo
bashgit clone https://github.com/Shardul-19/Mnist_CNN_99percent.git
cd Mnist_CNN_99percent
2. Install dependencies
bashpip install tensorflow matplotlib numpy
3. Run the notebook
bashjupyter notebook Mnist_CNN.ipynb

📊 Results
After 5 epochs of training on 48,000 samples (with 20% validation split):

Test Accuracy: ~99%
The model correctly identifies handwritten digits across all 10 classes
Predictions are visualized on 8 sample test images


🛠️ Tech Stack

Python 3.x
TensorFlow / Keras
NumPy
Matplotlib


📚 Dataset
MNIST — 70,000 grayscale images of handwritten digits (28×28 pixels)

Training set: 60,000 images
Test set: 10,000 images
Classes: 0–9 (10 classes)

Auto-downloaded via tensorflow.keras.datasets.mnist.

👤 Author
Shardul Rasal
B.Tech ENTC — Symbiosis Institute of Technology, Pune
GitHub

📄 License
This project is open source and available under the MIT License.
