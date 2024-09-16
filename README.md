# IMDB-Dataset-Analysis

Overview
This project focuses on analyzing IMDb movie data to extract meaningful insights about movies, directors, budgets, popularity, and other relevant information. The analysis includes SQL queries combined with Python's data manipulation libraries like Pandas to retrieve and explore data efficiently.

Project Structure
Notebook: IMDB_analysis.ipynb contains all the code for data analysis.
Data Source: The project queries IMDb data stored in a SQLite database to retrieve information on various aspects of movies.
Key Features
Director-specific Queries:

Analysis of movies directed by notable directors like Steven Spielberg.
Movie data such as title, budget, revenue, release date, popularity, and average votes are extracted.
Exploratory Data Analysis:

Data exploration and visualization of movie budgets, revenues, and popularity over time.
Movie ratings and their corresponding budgets are compared to identify patterns.
SQL Integration:

SQLite database is used to store and query movie-related data.
Complex SQL queries are used to filter, join, and retrieve specific information from the dataset.
DataFrames for Data Manipulation:

SQL query results are converted into Pandas DataFrames for easy manipulation and analysis.
Requirements
To run this project, ensure you have the following installed:
Python 3.x
Pandas
SQLite3
Matplotlib (for visualizations)
Installation
Clone the repository or download the notebook.
Install the required dependencies:
pip install pandas matplotlib sqlite3
Usage
Open the notebook IMDB_analysis.ipynb in Jupyter Notebook or any compatible editor.
Ensure you have the IMDb SQLite database connected correctly.
Run the cells to execute the analysis.
Example Queries
The project includes SQL queries such as:

SELECT m.Original_title, m.budget, m.popularity, m.Release_date, m.Revenue, m.vote_average
FROM movies AS m
JOIN directors AS d ON m.Director_id = d.id
WHERE d.name = 'Steven Spielberg';
This query retrieves details of movies directed by Steven Spielberg, including their budget, release date, and ratings.

Contributions
Feel free to fork this project and submit pull requests if you have any enhancements or suggestions.
