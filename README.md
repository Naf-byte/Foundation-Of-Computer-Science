📊 Trending YouTube Videos Analysis (2025–26 Project)

📌 Project Overview

This project analyzes the Trending YouTube Videos dataset across multiple countries.
The goal is to perform data cleaning, transformation, aggregation, and exploratory analysis using Python and Jupyter Notebook, following the requirements of the 2025–26 course project.

The project demonstrates practical skills in:

Data preprocessing

Feature engineering

Aggregations and grouping

Handling missing and invalid data

Working with CSV and JSON files

🛠️ Technologies Used

Python

Jupyter Notebook

Pandas

NumPy

JSON

(Any additional libraries used are documented inside the notebook)

📂 Dataset Description

The dataset consists of:

Multiple CSV files, each representing trending YouTube videos for a specific country

Multiple JSON files containing video category mappings

Each CSV file includes information such as:

Video title

Channel name

Views, likes, dislikes

Tags

Publish time

Trending date

Comment and rating status

📑 Project Tasks & Implementation

The following tasks were completed as part of this project:

Data Consolidation

All CSV files were concatenated into a single DataFrame.

A new column country was added to identify the source country.

Videos Without Tags

Extracted all videos that have no tags.

Total Views Per Channel

Computed the total number of views for each YouTube channel.

Excluded Videos

Created a new DataFrame called excluded containing:

Videos with disabled comments

Videos with disabled ratings

Videos marked as video_error_or_removed

These rows were removed from the main dataset.

Like Ratio Feature

Added a new column like_ratio calculated as:

likes / dislikes


Publish Time Clustering

Clustered publish times into 10-minute intervals
(e.g., 02:20–02:30).

Interval Analysis

For each time interval, calculated:

Number of videos

Average likes

Average dislikes

Tag Analysis

Extracted individual tags from the tag string.

Computed the number of videos per tag.

Most Frequent Tags

Identified tags with the largest number of videos.

Tag & Country Like Ratio

For each (tag, country) pair, computed the average like-to-dislike ratio.

Top Video by Views (Daily)

For each (trending_date, country) pair, identified the video with the highest views.

Trending Date Breakdown

Split trending_date into:

year

month

day

Top Video by Views (Monthly)

For each (month, country) pair, identified the video with the highest views.

Category Data Integration

Read all JSON files containing video categories.

Unassignable Categories

For each country, determined how many videos have categories that cannot be assigned.

🤖 Use of AI Tools

AI tools were used only as assistance for:

Understanding dataset structure

Clarifying Python/Pandas operations

Improving code readability

All logic, implementation, and explanations were fully reviewed and understood, and detailed explanations are provided directly in the notebook.

📁 Repository Structure
📦 Trending-YouTube-Analysis
 ┣ 📜 README.md
 ┣ 📓 Project_Notebook.ipynb
 ┣ 📂 data
 ┃ ┣ 📄 *.csv
 ┃ ┣ 📄 *.json

👥 Team Information

Group size: Up to 3 students

Group formation was done independently as per course guidelines.
