
# 🍷 Beverage Classifier using Decision Tree (from Scratch)

This project implements a basic **Decision Tree Classifier from scratch** in Python (using numpy) to classify beverages like **Beer, Wine, and Whiskey** based on their chemical properties.

---
📌 Features

- Decision Tree built using only `NumPy`
- Gini Impurity for best splits
- Manual recursive implementation of `build_tree()` and `predict()`
- Tree visualization using `matplotlib`
- Works on small numeric datasets

---

Functions Used

build_tree(x, y): Recursively builds the decision tree based on the provided features (x) and labels (y).
best_split(x, y): Finds the best feature and threshold using Gini impurity to split the dataset.
find_gini_impurity(labels): Calculates the Gini impurity for a set of labels, used to evaluate the quality of a split.
most_common_label(y): Finds the most frequent class label in the dataset, used for leaf nodes.
predict(node, x_test): Traverses the decision tree and predicts the class label for the input data point (x_test).
plot_tree(node): Visualizes the decision tree using matplotlib, plotting the tree structure.


Built as part of EPOCh Spring Camp session to understand decision trees from the ground up!

