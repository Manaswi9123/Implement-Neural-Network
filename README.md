# Implement-Neural-Network
# 🧠 Neural Network Implementation: From Scratch to TensorFlow

Have you ever wondered what happens inside a `model.fit()` call? This repository deconstructs the Artificial Neural Network (ANN) by building one from the ground up using Python and NumPy, providing a transparent view of how weights and biases are optimized.

---

## 🛠️ The Tech Stack
* **Language:** Python
* **Deep Learning Framework:** TensorFlow & Keras
* **Math & Data:** NumPy, Pandas
* **Visualization:** Matplotlib

---

## 🏗️ Core Architecture

### 1. The "From Scratch" Class (`myNN`)
I implemented a custom Python class that mimics the Keras Sequential API. It includes:
* **Fit Method:** Manages the training loop over specified epochs.
* **Gradient Descent Engine:** Manages the iterative updates of weights ($w_1, w_2$) and bias ($b$).
* **Log Loss Calculation:** Computes Binary Cross-Entropy to evaluate error.
* **Sigmoid Activation:** Squashes the weighted sum into a probability between 0 and 1.

### 2. The TensorFlow Benchmark
To ensure the custom implementation's accuracy, I built an equivalent single-neuron model in Keras:
* **Layer:** 1 Dense layer with Sigmoid activation.
* **Compilation:** Adam optimizer and `binary_crossentropy` loss.

---

## 🧪 Key Mathematical Implementations

The project focuses on the fundamental update rules of a neuron:
* **Weighted Sum:** $Z = w_1x_1 + w_2x_2 + b$
* **Activation:** $A = \frac{1}{1 + e^{-Z}}$
* **Cost Minimization:**
  $$w = w - \text{learning\_rate} \cdot \frac{\partial Loss}{\partial w}$$



---

## 📊 Results & Validation
By training on an insurance dataset, the "scratch" model and the "TensorFlow" model reached nearly identical final weights and biases.
* **Accuracy:** High performance on binary classification tasks.
* **Precision:** Verified by comparing prediction arrays from both implementations.

---

## 🚀 How to Run

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/Manaswi9123/Python-DataScience-Fundamentals.git](https://github.com/Manaswi9123/Python-DataScience-Fundamentals.git)

2. **Install Dependencies:**
    pip install tensorflow numpy pandas matplotlib

3. **Execute:** Run ImplementNN.ipynb to see the step-by-step comparison between the manual and automated approaches.
