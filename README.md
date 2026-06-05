# 🎬 Netflix Data Cleansing & Feature Engineering

## 📌 Project Overview
This project focuses on data cleansing and feature engineering using the global Netflix titles dataset. The main goal was to extract processable numeric metrics from mixed string columns (e.g., separating "90 min" from "2 Seasons") to calculate accurate business metrics.

## 🎯 Business Problem
In raw datasets, data types are often mixed. In this case, the `duration` column contained both minutes (for Movies) and seasons (for TV Shows). Business Intelligence tools cannot aggregate these strings directly without generating **False Positives** or errors.

## 🛠️ Cross-Tooling Solution
I solved this business problem using three different approaches to demonstrate technical versatility:

1. **Tableau:** Applied Row-Level Logic (`IF` statements) and String Manipulation (`SPLIT`) to create new calculated fields, separating Movies from TV Shows for an accurate tabular visualization.
2. **SQL:** Implemented `CASE WHEN` statements to conditionally parse strings and apply **Type Casting** (converting text to integers) directly at the query level.
3. **Python (Pandas):** Used Boolean Indexing (`np.where`) and vectorized operations to efficiently segregate the data in a DataFrame.

## 📈 Visual Output
Check out the Tableau dashboard tabular result here: 
> *(Cole aqui o link do Snipboard/ImgBB da sua captura de tela do Tableau)*

---
*Project built as part of my Data Analytics continuous learning journey.*
