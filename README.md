# 🎮 Game Recommendation System

A content-based recommendation engine suggesting similar games based on sales, user ratings, platforms, genres, and developer info.
**Approach**: Content-Based Filtering using TF-IDF and Cosine Similarity

---

## 📂 Repository Structure

- `3A.tsv` – Raw game dataset  
- `Game_Reccomendation.ipynb` – Main Jupyter notebook  
- `README.md` – Project documentation  

---

## 🔍 Dataset

The dataset (`3A.tsv`) contains detailed game marketplace information, including:

- **Basic info**: Name, Platform, Year_of_Release, Genre, Publisher, Developer, Rating  
- **Sales figures**: NA_Sales, EU_Sales, JP_Sales, Other_Sales, Global_Sales  
- **Review scores**: Critic_Score, Critic_Count, User_Score, User_Count  

These features are used to compute game similarity for content-based recommendations.

---

## 🛠️ Methodology

- **Data Preprocessing**: Handle missing values 
- **Feature Engineering**: Combine relevant features (Name, Platforms, Genres, Publisher) into unified text representation  
- **Recommendation Model**: TF-IDF vectorization + cosine similarity  
- **Recommendation Function**: Returns top 5 similar games for any given title  

---

## 🎯 Key Features

- Handles missing data intelligently  
- Combines multiple game attributes for robust similarity measurement  
- Provides clear and actionable recommendations  
- Returns informative messages for invalid or missing game queries  
