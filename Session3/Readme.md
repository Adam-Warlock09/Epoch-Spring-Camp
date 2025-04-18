# 📍 Indian Pincode Clustering — K-Means from Scratch

This project was developed to implement a complete **clustering pipeline from scratch** using the **K-Means algorithm**, grouping pincodes based on their **latitude and longitude** — with a specific focus on **West Bengal** (or one's own home state).

Built using only `NumPy`, `Pandas`, and basic visualization libraries, the project emphasizes careful geographical data filtering, algorithmic clarity, and insights drawn from unsupervised clustering techniques.

---

## 🗺️ Problem Statement

A dataset (`clustering_data.csv`) containing Indian pincodes with their geographic coordinates was provided. The task was defined as follows:

- The data had to be filtered to retain only entries from the **home state**
- A geographic plot of the pincodes was to be created
- A **K-Means Clustering algorithm** was to be implemented from scratch
- The **optimal number of clusters** had to be determined using the **Elbow Method**
- Final clusters had to be visualized clearly
- Inferences were to be drawn based on the output clusters

---

## 🧠 Key Features

- Filtering of data was performed based on **state name** (e.g., West Bengal)
- A custom implementation of **K-Means Clustering** was used
- Cluster results were visualized geospatially
- The **Elbow Method** was applied using Within-Cluster Sum of Squares (WCSS)
- **Second derivative logic** was used to auto-detect the elbow point
- The code was kept modular and clean
- Interpretations and observations were added based on clustering results

---

## 🔧 Core Functions

- `kmeans(X, k, max_iters=100)`: Implements the K-Means algorithm from scratch, returning centroids and labels
- `compute_wcss(X, centroids, labels)`: Calculates WCSS as a measure of clustering compactness
- `run_elbow_method(X)`: Runs clustering for a range of K values and returns WCSS for each
- `find_elbow_point(wcss_values)`: Detects the elbow using second derivative to suggest the optimal K
- `plot_clusters(X, labels, centroids)`: Plots clustered data, color-coded by cluster label

---

## 📈 Visualizations

The following visual outputs were created to support the analysis:

- **Scatter Plot** showing all pincodes in the selected state
- **Elbow Curve** to analyze WCSS across K values
- **Final Cluster Map** displaying grouped regions with distinct colors for each cluster

---

## 🧹 Preprocessing Steps

To prepare the data for clustering:

- Missing values and duplicates were removed
- Coordinate formats were standardized if necessary
- Accurate filtering was ensured using the state column
- Indexes were reset for clean plotting and computation

---

## 📊 Inference and Insights

From the final cluster visualization, several interpretations could be drawn. These included:

- Separation between **urban and rural pincode densities**
- Groupings influenced by **terrain or natural geography**
- Possible alignment with **administrative or planning zones**

These insights may be useful in tasks such as delivery route optimization, service distribution planning, or infrastructure development.

---

## 🚀 How to Run

Use `Unsupervised Learning Task.ipynb`