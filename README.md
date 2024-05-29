# Project Title
Movie Dataset Visualization
## Purpose
The purpose of this project is to analyze and visualize data from a movie dataset. By performing data cleaning and exploratory data analysis (EDA), we aim to uncover insights about the movie industry, such as trends in genres, box office performance, and ratings. This project serves as a comprehensive example of how to handle and extract meaningful information from a large dataset.
## Dataset
The dataset used in this project contains information about movies, including attributes such as title, genre, release date, budget, revenue, ratings, and more. The data was sourced from <[https://www.kaggle.com/datasets/rounakbanik/the-movies-dataset?select=movies_metadata.csv](https://www.kaggle.com/code/ibtesama/getting-started-with-a-movie-recommendation-system/input?select=movies_metadata.csv)>, and it includes records from 1920 to 2017.
## Tools and Libraries
This project was implemented using the following tools and libraries:
- Python
- Pandas
- NumPy
- Matplotlib
- Plotly
## Data Cleaning
<h3>movies_copy_1</h3>
- The dataset initially had 24 columns and 45,463 rows.
- Deleted 8 unwanted columns.
- Set the data types of three columns to the desired datatype (int) by exploring those columns and deleting the unwanted records.
- Checked for NaN values and deleted the records with NaN values because they accounted for less than 0.5% of the dataset.
- Changes were stored in <b>movies_copy_1.</b>
<br/>
<h3>movies_copy_2</h3>
- Deleted records where both the <b>budget</b> and <b>revenue</b> were zero to minimize redundancy.
- Kept only the <b>original_language</b> column and discarded the 'spoken language' column, as well as kept only the <b>title </b>column and discarded the 'original_title' column because they depicted the same values.
- Used the <b>literal eval </b> function to format the <b>production_companies</b> and <b>genre</b> columns due to improper formatting.
- Extracted <b>First_genre</b> and <b>Second_genre</b> from the <b>genre</b> column. 
- Extracted the <b>production_company</b> column from the <b>production_companies</b> column.
<br/>


