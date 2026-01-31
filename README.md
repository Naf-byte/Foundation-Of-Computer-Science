# 📊 Trending YouTube Videos Analysis (2025–26 Project)

## 📌 Project Overview
This project analyzes the **Trending YouTube Videos dataset** across multiple countries.  
The goal is to perform data cleaning, transformation, aggregation, and exploratory analysis using **Python and Jupyter Notebook**, following the requirements of the 2025–26 course project.

The project demonstrates practical skills in:
- Data preprocessing  
- Feature engineering  
- Aggregations and grouping  
- Handling missing and invalid data  
- Working with CSV and JSON files  

---

## 🛠️ Technologies Used
- **Python**
- **Jupyter Notebook**
- **Pandas**
- **NumPy**
- **JSON**

---

## 📂 Dataset Description
The dataset consists of:
- Multiple **CSV files**, each representing trending YouTube videos for a specific country  
- Multiple **JSON files** containing video category mappings  

Each CSV file includes information such as:
- Video title  
- Channel name  
- Views, likes, dislikes  
- Tags  
- Publish time  
- Trending date  

---

## 📑 Project Tasks & Implementation

1. Created a single DataFrame by concatenating all CSV files and added a `country` column.
2. Extracted all videos with no tags.
3. Computed the total number of views for each channel.
4. Saved videos with disabled comments, disabled ratings, or marked as `video_error_or_removed` into a new DataFrame called `excluded`, and removed them from the main dataset.
5. Added a `like_ratio` column calculated as likes divided by dislikes.
6. Clustered publish times into **10-minute intervals**.
7. For each interval, calculated the number of videos, average likes, and average dislikes.
8. Extracted individual tags and determined the number of videos per tag.
9. Identified tags with the largest number of videos.
10. Computed the average like-to-dislike ratio for each `(tag, country)` pair.
11. Found the video with the highest number of views for each `(trending_date, country)` pair.
12. Split `trending_date` into `year`, `month`, and `day`.
13. Found the video with the highest number of views for each `(month, country)` pair.
14. Read all JSON files containing video categories.
15. Determined how many videos per country have categories that are not assignable.

---

## 🤖 Use of AI Tools
AI tools were used to assist with:
- Understanding dataset structure  
- Clarifying Pandas operations  
- Improving code readability  

All analysis and logic were fully reviewed and understood, with explanations provided in the notebook.

---

## 📁 Repository Structure
Trending-YouTube-Analysis/
│

├── README.md

├── Project_Notebook.ipynb

└── data/

├── *.csv
└── *.json

