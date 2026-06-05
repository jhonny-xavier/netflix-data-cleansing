# 🎬 Netflix Data Cleansing & Exploratory Data Analysis (EDA)

## 📌 Project Overview
This project focuses on **End-to-End Data Analysis**, starting with data cleansing and feature engineering, culminating in a comprehensive Business Intelligence Dashboard using the global Netflix titles dataset.

## 🎯 Business Problem & Solution
The raw dataset contained mixed string columns (e.g., `duration` had both "90 min" and "2 Seasons"). I applied conditional logic to extract processable numeric metrics to avoid **False Positives** during aggregation.

### 🛠️ Cross-Tooling Approach:
1. **Tableau:** Applied Row-Level Logic (`IF`) and String Manipulation (`SPLIT`) to segregate Movies from TV Shows.
2. **SQL:** Implemented `CASE WHEN` statements to conditionally parse strings and apply Type Casting.
3. **Python (Pandas):** Used Boolean Indexing (`np.where`) and vectorized operations for efficient dataframe segregation.

## 📊 Exploratory Data Analysis & Dashboard
Once the data was cleaned, I conducted an EDA to answer key business questions:
- **Geospatial Analysis:** Where is our content coming from? *(Symbol Map)*
- **Time-Series Trend:** How has production grown over the years? *(Line Chart)*
- **Market Share:** What is the proportion of Movies vs. TV Shows? *(Pie Chart)*
- **Top N Categories:** Which genres dominate the platform? *(Bar Chart)*

### ✨ Final Dashboard Visual
*(Substitua o texto abaixo pela imagem do seu dashboard. Pode arrastar a imagem diretamente do seu computador para dentro desta caixa de edição do GitHub e ele gera o código automaticamente)*
[<img width="1363" height="764" alt="Dash" src="https://github.com/user-attachments/assets/421eaf92-9d22-44ec-a6c2-6d6943429049" />
]

---
*Project built as part of my Data Analytics continuous learning journey.*
