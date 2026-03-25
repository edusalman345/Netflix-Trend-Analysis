# 📊 Netflix Data Analysis

## 📌 Project Overview

This project analyzes the Netflix dataset to understand content distribution and identify the most popular genres available on the platform. The analysis focuses on cleaning raw data, extracting meaningful insights, and presenting them through visualization.

---

## 🎯 Objectives

* Analyze the Netflix dataset
* Identify top genres
* Visualize content trends
* Present insights in a simple and clear way

---

## 🗂️ Dataset

The dataset includes:

* Title
* Type (Movie / TV Show)
* Genre (`listed_in`)
* Release Year
* Country
* Description

---

## 🧹 Data Cleaning

To ensure accurate results, the following steps were performed:

* Split multiple genres into individual values
* Removed extra spaces (e.g., `"Dramas"` vs `" Dramas"`)
* Standardized genre formatting

```python
genres = (
    df['listed_in']
    .str.split(',')
    .explode()
    .str.strip()
)
```

---

## 📊 Analysis & Findings

### 🔝 Top Genres

* International Movies dominate the platform
* Dramas and Comedies are highly popular
* Other genres like Documentaries and Action & Adventure show moderate presence

---

## 📈 Visualization

A bar chart was created to display the top 10 genres.

### 📌 Key Insight

Netflix focuses heavily on **international and story-driven content**, indicating a strategy aimed at a **global audience** while maintaining content variety.

---

## 🛠️ Tools & Technologies

* Python
* Pandas
* Matplotlib

---

## 📁 Project Structure

```
netflix-data-analysis/
│── netflix_analysis.ipynb
│── top_genres.csv
│── README.md
```

---

## 🚀 Future Improvements

* Analyze trends over time (release year)
* Compare Movies vs TV Shows
* Country-wise analysis
* Build interactive dashboard (Power BI / Streamlit)

---

## 👨‍💻 Author

Ahmad Salman

---

## ⭐ How to Use

1. Clone the repository
2. Open the notebook in Jupyter/Colab
3. Run all cells to reproduce the analysis

---

## 📌 Conclusion

This project demonstrates how raw data can be transformed into meaningful insights through cleaning, analysis, and visualization. It highlights Netflix’s strong focus on international and drama-based content.
