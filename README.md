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
1. Dataset has 24 columns and 45463 rows.
2. Deleted the unwanted 8 columns.
3. Set the datatypes of three columns to desired datatype (int) by doing exploration of those columns and by deleting the unwanted records from those columns.
4. Checked the NAN values Deleted the records od NAN values because the NAN records were less than 0.5%.
5. Changes are stored in df_copy_1.
<br/>
<h3>movies_copy_2</h3>
1. Deleted the records where the 'budget' and 'revenue' both were zero to minimize the redudancy.
2. From the columns 'original language' and 'spoken language' only the column 'original language' kept and from 'original_title' and 'title' only the 'title' column is kept because both were depicting the same values.
3. <b>literal eval </b>function is used to format the columns <b>production_companies</b> and <b>genre</b> because these columns have improper formatting. 
4. Extracted <b>First_genre</b> and <b>Second_genre</b> from the <b>genre</b> column. 
5. Extracted the <b>production_company</b> column from the <b>production_companies</b> column.
<br/>

