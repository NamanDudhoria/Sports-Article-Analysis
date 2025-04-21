# 📰 Sports Articles Analysis 

## 📌 Overview
This project explores unsupervised learning techniques to analyze sports-related media articles from December to March. It aims to discover patterns in article structure, timing, platform, and athlete mentions using feature engineering and KMeans clustering.

---

## 📂 Files in the Repo
- `1dec - 31st march.xlsx`: Main dataset containing article metadata.
- `players.xlsx`: List of athlete names used for tagging.
- `Sports.ipynb`: Data loading, feature engineering, and EDA.
- `sports_clustering.ipynb`: KMeans clustering pipeline and analysis.
- `visualizations/`: Saved cluster plots and summary charts.
- `Sports_Media_Clustering_Report.pdf`: Final report in PDF format.
- `README.md`: This file.

---

## ✨ Key Features

### 🔧 Feature Engineering
- **Temporal Features**: Weekday and time-of-day bins.
- **Textual Features**: Title length, word count, presence of numbers, questions, or quotes.
- **Player Tagging**: Articles matched with athlete names from a curated list.
- **One-Hot Encoding**: Categorical columns transformed for modeling.

### 📉 Regression Attempts
- Applied multiple models (Lasso, Elastic Net, Random Forest, etc.) using TF-IDF and SentenceTransformer embeddings.
- All regression models showed poor predictive power (R² ≈ 0), leading to a pivot toward clustering.

---

## 🔁 Clustering Approach

### Algorithm Used
- **KMeans Clustering**
- Optimal cluster count determined using **Silhouette Score** and **Inertia**.
- Final clusters: **3** (after merging low-frequency/low-impact subgroups).


## 📉 Limitations & Future Work
- Player tagging based on substring match — can be improved with NLP/NER.
- Article **body content** not analyzed — future could include embeddings.
- Consider **platform-specific clustering** for targeted strategy.

---

## 📄 License
This project is open for educational use. Please cite or credit when used.

---

## 🙌 Acknowledgements
Developed by [Naman Dudhoria], powered by `pandas`, `scikit-learn`, `seaborn`, `sentence-transformers`, and `pycaret`.


