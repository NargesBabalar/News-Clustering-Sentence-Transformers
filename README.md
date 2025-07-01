# 📰 News Clustering using Sentence Transformers & Clustering Algorithms

This project tackles the **unsupervised clustering** of news articles using semantic embeddings from a pretrained transformer model and traditional clustering techniques.  
The goal is to group articles based on **semantic similarity**, enabling automatic **topic discovery** and large-scale text organization.

> 🎓 **Course**: Artificial Intelligence  
> 🏛️ **University**: University of Tehran – School of Electrical & Computer Engineering  
> 👨‍🏫 **Instructor**: Dr. YaghoobZadeh  

---

## 🎯 Objectives

- Extract contextual embeddings using **all-MiniLM-L6-v2** from Sentence Transformers  
- Apply and compare clustering algorithms:
  - K-Means
  - DBSCAN
  - Hierarchical Clustering
- Evaluate clustering results with:
  - **Silhouette Score**
  - **Homogeneity Score**
- Visualize semantic space using **PCA** (2D projection)

---

## 🔄 Workflow Overview

### 1️⃣ Data Preprocessing:
- Text normalization:
  - Lowercasing  
  - Stop word removal  
  - Punctuation stripping  
- (Optional): Lemmatization / stemming

### 2️⃣ Embedding Extraction:
- Model: `sentence-transformers/all-MiniLM-L6-v2`  
- Output: 384-dimensional semantic vectors  

### 3️⃣ Clustering Techniques:
- **K-Means**:
  - Optimal `k` via Elbow Method  
- **DBSCAN**:
  - Density-based; handles outliers well  
- **Agglomerative Clustering**:
  - Hierarchical structure; dendrogram interpretation  

### 4️⃣ Dimensionality Reduction:
- **PCA** used to project embeddings into 2D space  
- Enables **visual clustering diagnostics**

---

## 📊 Evaluation Metrics

| Metric             | Description                                         |
|-------------------|-----------------------------------------------------|
| **Silhouette Score** | Measures intra-cluster cohesion vs inter-cluster separation |
| **Homogeneity Score** | Checks if clusters contain only one class type      |

---

## 🔍 Key Insights

- Sentence-BERT (`MiniLM`) provides **powerful semantic embeddings**  
- **K-Means** yielded the most distinct, interpretable clusters  
- **DBSCAN** effectively isolated **noisy articles** and **small clusters**  
- **PCA visualizations** helped validate and interpret clustering patterns

---

## 🛠 Tools & Libraries

- **Python** (Jupyter Notebook)  
- `sentence-transformers`  
- `scikit-learn`  
- `matplotlib`, `seaborn`  
- `pandas`, `numpy`

---

> 💡 This project demonstrates the synergy between **transformer-based NLP** and **unsupervised learning** in organizing and interpreting large-scale text datasets.
