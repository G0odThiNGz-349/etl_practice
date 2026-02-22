
TMDB Movies ETL Pipeline (2021–2025)
This project demonstrates an ETL (Extract, Transform, Load) pipeline that processes movie data from TMDB (2021–2025) and loads it into a MySQL data warehouse
 ------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Project Overview:
Goal: Build a data warehouse to analyze movie statistics, genres, and ratings.
Dataset: tmdb_movies_2021_2025.csv containing movies with metadata like title, release date, overview, genre, and ratings.

Pipeline Steps:
Extract – Load the CSV dataset into Pandas.
Transform – Clean missing data, handle genres, and prepare dimension & fact tables.
Load – Store data in MySQL using SQLAlchemy, creating a star schema.

Star Schema Design:
<img width="1024" height="1536" alt="etl" src="https://github.com/user-attachments/assets/2a238b75-6bbb-48aa-872c-efbb7d93b510" />


🛠 Technologies Used:
Python 3.9+
Pandas – Data cleaning & transformation
SQLAlchemy – MySQL integration & schema creation
MySQL – Relational data warehouse
dotenv – Secure environment variable management


Data Cleaning & Transformation Highlights:
Dropped movies with missing title or tmdb_id.
Filled missing overview with "No overview available".
Exploded multiple genres into a bridge table to handle many-to-many relationships.


This project demonstrates the ability to:
Handle real-world messy datasets
Design a star schema for analytics
Write Python ETL scripts with Pandas
Use SQLAlchemy to interact with a relational database
Prepare data for business intelligence or analytics dashboards
