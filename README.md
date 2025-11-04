# 🎬 Movie Revenue Correlation using Python  

![Python](https://img.shields.io/badge/Python-3.10%2B-blue?logo=python)
![Jupyter](https://img.shields.io/badge/Notebook-Jupyter-orange?logo=jupyter)
![EDA](https://img.shields.io/badge/EDA-Exploratory_Data_Analysis-green)
![License](https://img.shields.io/badge/License-MIT-yellow)

---

## 🧠 Overview  
An end-to-end **Exploratory Data Analysis (EDA)** project that explores which factors contribute most to a movie’s box office success.  
Using a public **Kaggle dataset**, I cleaned, transformed, and visualized movie data to uncover the relationships between **budget**, **gross earnings**, and other attributes like **rating**, **company**, and **genre**.

---

## 🎯 Objective  
Film studios and data analysts often want to understand:  
> “What makes a movie financially successful?”  

This project aims to:  
- Clean and preprocess movie metadata for reliability.  
- Quantify correlations between film attributes and gross revenue.  
- Visualize insights using modern Python data analysis libraries.  

---

## 📊 Dataset  
| Property | Description |
|-----------|-------------|
| **Source** | [Kaggle Movie Dataset](https://www.kaggle.com/datasets/danielgrijalvas/movies) |
| **Rows** | 7,669 (after cleaning) |
| **Columns** | 15 |
| **Period** | 1986 – 2019 |
| **Key Features** | Title, Budget, Gross, Company, Genre, Rating, Runtime, Release Date |

---

## 🧰 Tech Stack  
| Tool | Purpose |
|------|----------|
| **Python** | Core programming language |
| **Pandas / NumPy** | Data wrangling and transformations |
| **Matplotlib / Seaborn** | Data visualization and regression plots |
| **Jupyter Notebook** | Interactive development environment |

---

## 🔍 Approach  
1. **Data Loading & Inspection**  
   - Imported the Kaggle dataset using Pandas.  
   - Reviewed schema, missing values, and datatypes.

2. **Data Cleaning & Preparation**  
   - Fixed incorrect datatypes and inconsistent formats.  
   - Created a `year` column from release dates.  
   - Removed duplicates, handled missing values, and normalized numeric fields.  
   - Trimmed extreme outliers to prevent skewed correlations.

3. **Exploratory Analysis**  
   - Generated descriptive statistics and plotted data distributions.  
   - Analyzed categorical and numerical variables individually.

4. **Correlation Analysis**  
   - Used **Pearson correlation** for numerical variables.  
   - Applied **label encoding** for categorical columns (`studio`, `rating`, `genre`).  
   - Compared pre- and post-encoding correlation matrices.  
   - Visualized relationships using **heatmaps, scatter, and regression plots**.

---

## 📈 Key Findings  
| Insight | Observation |
|----------|--------------|
| 💰 **Budget ↔ Gross** | Strong positive correlation (**r ≈ 0.75**) |
| 🕐 **Year Released** | Moderate correlation — newer films earn slightly more |
| 🎞 **Genre & Rating** | Certain genres (Action, Adventure) and ratings (PG-13) dominate higher revenue |
| ⚠️ **Outliers** | High-budget films show diminishing returns beyond a threshold |

---

## 🖼 Visualizations  

| Visualization | Description |
|----------------|-------------|
| ![Budget vs Gross](./images/movie-scatter-budget-gross.png) | Scatter plot with regression line showing `Budget` vs `Gross` |
| ![Correlation Heatmap](./images/movie-corr-heatmap.png) | Pearson heatmap of all numerical and encoded categorical features |
| ![Top Factors](./images/movie-top-factors.png) | Top correlated features influencing gross revenue |

---

## ⚙️ How to Run  

### 1️⃣ Clone the Repository  
```bash
git clone https://github.com/Filazion/movie-revenue-correlation.git
cd movie-revenue-correlation
