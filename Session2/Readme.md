# 🍏🥃 ML Classifiers from Scratch — KNN & Decision Tree

This project showcases two classic machine learning classifiers — implemented **from scratch** using only **Python** and **NumPy**. These models are built to classify:

- 🍎 Fruits (Apple, Banana, Orange) using **K-Nearest Neighbors (KNN)**
- 🥃 Beverages (Beer, Wine, Whiskey) using a **Decision Tree**

Both implementations are designed for learning and conceptual clarity — no external ML libraries like `scikit-learn` are used.

---

## 🧠 Implemented Models

### 🔹 1. K-Nearest Neighbors (KNN) — Fruit Classifier

Classifies fruits based on **weight**, **size**, and **color**.

#### 📌 Features
- Built using only `NumPy`
- Calculates **Euclidean distance** for similarity
- Uses **majority voting** to decide the predicted class
- Custom `KNN` class with methods: `fit`, `predict`, `predict_one`
- Configurable `k` (number of neighbors)
- Toy dataset included for experimentation

#### 🔧 Key Functions
- `euclidean_distance(x1, x2)`: Distance metric
- `KNN(k=3)`: Classifier with `fit`, `predict`, and `predict_one`
- `label_encoding` & `data_preprocessing`: Converts string labels into numeric form and separates features from labels

#### 🧪 Testing
- Evaluate predictions on test samples with known expected outcomes
- Try different `k` values to observe prediction changes

---

### 🔸 2. Decision Tree — Beverage Classifier

Classifies beverages based on chemical properties using a decision tree built with **Gini impurity**.

#### 📌 Features
- Recursive decision tree construction
- Uses **Gini impurity** to select optimal feature-threshold splits
- Custom tree nodes (internal and leaf)
- Full implementation of prediction logic
- Visualizes tree using `matplotlib` (optional)
- Works on numeric datasets

#### 🔧 Key Functions
- `build_tree(x, y)`: Builds the decision tree recursively
- `best_split(x, y)`: Finds best feature and threshold
- `find_gini_impurity(labels)`: Measures impurity of a split
- `most_common_label(y)`: Used for leaf nodes
- `predict(node, x_test)`: Traverses the tree to predict class label
- `plot_tree(node)`: Visualizes the tree using `matplotlib`

---

## 🚀 How to Run

### Requirements
- Python 3.x
- NumPy

### Running KNN Classifier

```bash
python knn_classifier.py
