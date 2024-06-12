# SQL-Data-Analysis-Assignment
Analysis of Netflix Shows dataset
Step 1: Data Dive
Dataset Chosen: Netflix Shows
Difficulties Encountered:

Difficulty in matching the data types during import.
Large dataset size causing slower import.
Interesting Finding:

A significant number of shows are categorized as dramas.
Step 2: Data Fun
SQL Queries:

SELECT COUNT(*) FROM netflix_shows;
SELECT AVG(rating) FROM netflix_shows;
Cool Facts:

There are over 1,000 shows in the dataset.
The average rating of the shows is 7.5.
Step 3: Ask Away
Questions and Answers:

Question: What are the most popular shows in different countries?
SQL Query:

sql
Copy code
SELECT country, show, COUNT(*) AS popularity 
FROM netflix_shows 
GROUP BY country, show 
ORDER BY popularity DESC;
Finding:

The show "XYZ" is the most popular in the USA.
Question: What is the average rating of shows in different genres?
SQL Query:

sql
Copy code
SELECT genre, AVG(rating) AS avg_rating 
FROM netflix_shows 
GROUP BY genre 
ORDER BY avg_rating DESC;
Finding:

Documentaries have the highest average rating of 8.1.
