# Deep Learning Fashion Image Classification

## 📌 Project Overview

This project demonstrates how **Deep Learning** can be used to automatically classify fashion product images into different categories.

The project is based on a practical **e-commerce business scenario**, where an online fashion company receives thousands of product images and wants to reduce repetitive manual work involved in product categorization.

A Neural Network is trained using the **Fashion-MNIST dataset** to identify the category of a fashion product image.

---

## 🏢 Business Problem

An e-commerce company receives a large number of product images every day.

Currently, employees manually identify and select the category of each product before adding it to the website.

This process can be:

* Time-consuming
* Repetitive
* Difficult to scale
* Inconsistent when handling large numbers of products

The company wants to use **AI and Deep Learning** to assist employees with automatic product categorization.

---

## 🤖 AI Solution

A Deep Learning model analyzes a product image and predicts its category.

### Process

**Product Image → Deep Learning Model → Predicted Category → Human Review → Website**

The model learns patterns from labelled fashion images and uses those patterns to classify new images.

---

## 👗 Product Categories

The model classifies images into **10 categories**:

1. T-shirt / Top
2. Trouser
3. Pullover
4. Dress
5. Coat
6. Sandal
7. Shirt
8. Sneaker
9. Bag
10. Ankle Boot

These categories are defined in the notebook.

---

## 📊 Dataset

The project uses the **Fashion-MNIST** dataset.

The dataset contains grayscale images of common fashion products and is downloaded automatically through TensorFlow/Keras.

Each image is processed before being given to the neural network.

---

## 🧠 Model Architecture

The project uses a simple Artificial Neural Network.

### Architecture

```text
Input Image
     ↓
Flatten Layer
     ↓
Dense Layer - 64 Neurons
     ↓
ReLU Activation
     ↓
Output Layer - 10 Classes
     ↓
Softmax
     ↓
Predicted Product Category
```

The notebook uses:

* `Flatten` layer
* `Dense(64)` hidden layer
* `ReLU` activation
* `Dense(10)` output layer
* `Softmax` activation

The 10 output neurons represent the 10 fashion categories.

---

## 🛠️ Technologies Used

* **Python**
* **TensorFlow**
* **Keras**
* **NumPy**
* **Matplotlib**
* **Google Colab**
* **Fashion-MNIST**

---

## 🔄 Project Workflow

### 1. Import Libraries

TensorFlow, NumPy and Matplotlib are imported.

### 2. Load Dataset

Fashion-MNIST training and testing images are loaded.

### 3. Define Categories

The numerical labels are connected with understandable product names.

### 4. Visualize Images

Sample fashion product images are displayed.

### 5. Data Preparation

Pixel values are normalized from `0–255` to `0–1`.

### 6. Build Neural Network

A simple neural network is created using TensorFlow/Keras.

### 7. Compile Model

The model is compiled using the Adam optimizer, categorical cross-entropy loss and accuracy as the evaluation metric.

### 8. Train Model

The neural network is trained for 3 epochs with a validation split.

### 9. Evaluate Model

The trained model is tested using images that were not used during training.

### 10. Make Predictions

The model predicts the category of new fashion images.

This complete workflow is implemented in the notebook.

---

## 📈 Model Evaluation

The model is evaluated using **test accuracy**.

The exact accuracy can vary depending on the training run. The notebook explains accuracy as the percentage of test images that are classified correctly.

> **Note:** Accuracy alone should not be the only consideration before deploying an AI system. Incorrect classifications, customer experience, training-data quality and human review should also be considered.

---

## 💼 Business Application

This project can be applied to a fashion e-commerce platform.

### Traditional Process

```text
Product Image
     ↓
Employee manually selects category
     ↓
Product added to website
```

### AI-Assisted Process

```text
Product Image
     ↓
Deep Learning Model
     ↓
Predicted Category
     ↓
Employee Review
     ↓
Product added to website
```

The notebook identifies potential benefits such as faster product listing, reduced repetitive manual work, more consistent categorization and improved product-search experience.

---

## 🎯 Business Benefits

Possible benefits include:

* Faster product listing
* Reduced repetitive manual work
* More consistent product categorization
* Better product-search experience
* Ability to process a larger number of images

---

## ⚠️ Limitations

The model may sometimes classify an image incorrectly.

Therefore, a human employee can remain involved in situations where:

* The prediction is uncertain
* The product category is important
* An incorrect classification could affect customers
* The image is different from the training data

The project emphasizes that AI predictions are not always correct and that businesses should consider human oversight.

---

## 📁 Repository Structure

```text
deep-learning-fashion-image-classification/
│
├── part-a/
│   └── deep-learning/
│       └── Deep_Learning_Fashion_Classification_Name.ipynb
│
├── README.md
│
└── screenshots/
    └── prediction.png
```

---

## 🚀 How to Run the Project

### Option 1: Google Colab

1. Open the `.ipynb` notebook in Google Colab.
2. Run the cells from top to bottom.
3. The Fashion-MNIST dataset will download automatically.
4. Train the model.
5. Check the test accuracy.
6. Try different image numbers to see predictions.

### Option 2: Jupyter Notebook

Install the required libraries:

```bash
pip install tensorflow numpy matplotlib
```

Then open the notebook and run the cells.

---

## 🔮 Future Improvements

The current project uses a simple Artificial Neural Network.

Future versions could explore:

* Convolutional Neural Networks (CNN)
* Data augmentation
* Larger/deeper models
* Confusion matrix
* Precision, recall and F1-score
* Confidence scores
* Real-world fashion product images
* Web application for image upload and prediction
* Human-in-the-loop review system

---

## 🎓 Learning Outcomes

Through this project, students learn:

* How images can be used as Deep Learning input
* Basic Artificial Neural Network architecture
* Input, hidden and output layers
* Image preprocessing
* Model training
* Model evaluation
* Image classification
* Business applications of AI
* Importance of human oversight

These learning objectives are part of the original practical.

---

## 📌 Project Type

**Domain:** Artificial Intelligence / Machine Learning
**Industry:** E-commerce / Fashion Technology
**Technique:** Deep Learning
**Task:** Image Classification
**Dataset:** Fashion-MNIST
**Framework:** TensorFlow / Keras
**Platform:** Google Colab
**Language:** Python

---

## 👩‍💻 Author

**Kamalpreet Kaur**

BBA FinTech AI

---

## ⭐ Conclusion

This project demonstrates how Deep Learning can help an e-commerce business automatically classify fashion product images.

Instead of completely replacing employees, the system can be used as an **AI-assisted classification tool**, where the model provides a prediction and employees can review the result when required.
