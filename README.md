# IRIS_FLOWER_PREDICTION_USING_CNN


# 🌸 Iris Flower Prediction Using CNN (Deep Learning)

This project applies **Convolutional Neural Networks (CNN)** to classify **Iris flowers** into three species: **Setosa**, **Versicolor**, and **Virginica**. While traditional ML algorithms are common for this dataset, this project uniquely leverages **deep learning** to demonstrate CNN capabilities even on structured data.

---

## 📌 About the Project

The **Iris dataset** is a classic classification problem in machine learning. This project:
- Uses a **1D CNN** model to classify flower species
- Converts tabular features into a suitable shape for CNNs
- Trains a deep learning model using **TensorFlow/Keras**
- Visualizes training accuracy and loss

This is a great demonstration of applying CNNs to non-image datasets by reshaping data appropriately.

---

## 🔍 Features of the Project

- Uses the `Iris` dataset from `sklearn.datasets`
- Preprocesses the data and reshapes it to fit CNN input shape
- One-hot encoding for categorical output
- Trains a CNN model with:
  - Conv1D + MaxPooling1D layers
  - Dense output with Softmax activation
- Plots training history (accuracy & loss)
- Predicts flower species based on user-defined input

---

## 🌺 Iris Dataset Info

Each sample includes the following features:
- `sepal_length`
- `sepal_width`
- `petal_length`
- `petal_width`

Target classes:
- `Setosa`
- `Versicolor`
- `Virginica`

---

## 🧠 Model Architecture

The CNN model includes:

- Input Layer reshaped as `(4, 1)` for Conv1D
- `Conv1D` Layer (filters = 64, kernel_size = 2, activation = 'relu')
- `MaxPooling1D` Layer
- `Flatten` Layer
- `Dense` Layer (units = 32, activation = 'relu')
- Output `Dense` Layer (units = 3, activation = 'softmax')

---

## 📈 Evaluation

- **Training Accuracy:** ~99% (varies by run)
- Loss and accuracy plots provided for visual evaluation
- Final model can predict the correct flower class based on input features

---

## 🚀 How to Run

1. Open the notebook in Google Colab or Jupyter
2. Run all cells sequentially
3. Use the test cell to input custom flower measurements for prediction

### 🧪 Example Input
```python
test_input = np.array([[5.1, 3.5, 1.4, 0.2]])
Predicted Flower Class: Setosa

