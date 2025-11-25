-----

## ✍️ MNIST Handwritten Digit Classification using Deep Neural Networks

A simple yet effective implementation of a **Deep Neural Network (DNN)** to accurately classify handwritten digits from the **MNIST dataset**. This project serves as an excellent introduction to image classification using foundational concepts in deep learning with **TensorFlow/Keras**.

-----

## ✨ Features

  * **MNIST Dataset:** Utilizes the canonical 60,000 training and 10,000 testing images of 28x28 grayscale handwritten digits.
  * **Simple DNN Architecture:** A straightforward network composed of an **Input Layer**, two **Dense Hidden Layers** with **ReLU** activation, and an **Output Layer** with **Sigmoid** activation.
  * **High Accuracy:** Achieves a **Test Accuracy** of approximately **97.02%**.
  * **Comprehensive Evaluation:** Includes training loss, test loss, and a **Confusion Matrix** analysis.

-----

## 🛠️ Prerequisites

Make sure you have the following installed:

  * **Python 3.x**
  * **Jupyter Notebook** or **Google Colab** 

You'll need the following libraries, which you can install via `pip`:

```bash
pip install numpy matplotlib seaborn tensorflow keras
```

-----

## 📂 Project Structure

The core of the project is contained within a single notebook, but the overall setup is simple:

```
.
├── MNIST_Classification_DNN.ipynb  # Main notebook with all code
├── README.md                       # This file
└── ...                             # Other potential files 
```

-----

## 🧠 Model Architecture Overview

The model is built using the `Sequential` API in Keras:

| Layer | Type | Output Shape | Activation Function | Purpose |
| :--- | :--- | :--- | :--- | :--- |
| **1 (Input)** | `Flatten` | (28 \* 28) = 784 | N/A | Flattens the 2D image into a 1D vector. |
| **2 (Hidden 1)**| `Dense` | 50 | `relu` | First fully connected hidden layer. |
| **3 (Hidden 2)**| `Dense` | 50 | `relu` | Second fully connected hidden layer. |
| **4 (Output)** | `Dense` | 10 | `sigmoid` | Outputs probability scores for the 10 classes (digits 0-9). |

  * **Loss Function:** `sparse_categorical_crossentropy` (used because the labels are integers, not one hot encoded).
  * **Optimizer:** `adam`
  * **Training:** Run for **10 epochs**.

-----

## ⚙️ How to Run

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/AmrElhady1/Handwritten_Digit_Classification.git
    cd Handwritten_Digit_Classification
    ```
2.  **Open the notebook:**
    Open `Handwritten_Digit_Classification.ipynb` in a Jupyter environment or Google Colab.
3.  **Execute Cells:** Run all the code cells sequentially. The notebook handles data loading, preprocessing, model definition, training, and evaluation automatically.

-----

## 📊 Results

The training demonstrated rapid convergence, yielding strong results:

  * **Training Accuracy:** **98.70%**
  * **Test Accuracy:** **97.02%**

The final evaluation is represented by the **Confusion Matrix**, which clearly shows which digits the model successfully predicted (diagonal) and which it misclassified (off-diagonal).

-----


<!-- This is an empty README file for the MNIST project -->
