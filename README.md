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
1. The dataset initially had 24 columns and 45,463 rows. <br/>
2. Deleted 8 unwanted columns. <br/>
3. Set the data types of three columns to the desired datatype (int) by exploring those columns and deleting the unwanted records.<br/>
4. Checked for NaN values and deleted the records with NaN values because they accounted for less than 0.5% of the dataset. <br/>
5. Changes were stored in <b>movies_copy_1.</b> <br/>
<br/>
<h3>movies_copy_2</h3>
1. Deleted records where both the <b>budget</b> and <b>revenue</b> were zero to minimize redundancy. <br/>
2. Kept only the <b>original_language</b> column and discarded the 'spoken language' column, as well as kept only the <b>title </b>column and discarded the 'original_title' column because they depicted the same values. <br/>
<br/>
<h3>movies_copy_3</h3>
3. Used the <b>literal eval </b> function to format the <b>production_companies</b> and <b>genre</b> columns due to improper formatting.<br/>
4. Extracted <b>First_genre</b> and <b>Second_genre</b> from the <b>genre</b> column. <br/>
5. Extracted the <b>production_company</b> column from the <b>production_companies</b> column.<br/>
<br/>
<h3>movies_copy_4</h3>
1. Checked the NaN values in the dataset. The counts are as follows <br/>
<ul>
<li><b>runtime</b> = 1</li>
<li> <b>first_genre</b> = 12</li>
<li> <b>second_genre</b> = 951 </li>
<li> <b>production_company</b> = 18 </li> </ul> <br/>
2. Some of the initial DataFrame records for <b>production_companies</b> and <b>genres</b> had empty lists. After applying literal_eval, these empty lists were converted to NaN. <br/>
3. Filled the NaN values in the <b>production_company</b> column using a Random Forest classifier. <br/>
4. Deleted the record where the <b>runtime</b> had a NaN value. <br/>
5. Filled the NaN values in the <b>second_genre</b> column using the ffill method, duplicating the <b>first_genre</b> values in the <b>second_genre</b> column where NaN values were present. <br/>
6. Deleted the 12 records where <b>first_genre</b> had NaN values. <br/>
7. Stored the dataframe to new location <b>cleaned_movie_data</b>
<br/>
# EDA: Exploratory Data Analysis
The Following Graphs are plotted,
<ul>
<li><b>Popular Genres Based on Popularity Score</b></li>
<li> <b>Movie Count by Genre: A Cinematic Breakdown</b> </li>
<li> <b>A Financial Journey Through Cinema from 1960 to 2017</b> </li>
<li> <b>Exploring Profits Based on First Genre</b> </li> 
<li><b>High Profit top 10 Movies/b></li>
<li><b>Popular Genres Based on Popularity Score</b></li>
<li><b>Movie count and Profit Analysis (For Production Companies)</b></li>
<li><b>Popular Genres Based on Popularity Score</b></li>
<li><b>Number of Movies Released Per Year Over Time</b></li>
<li><b>Deep Inside Movie Runtime</b></li>
<li><b>Influence of languages in Cinematics</b></li>
</ul> <br/>
<p>
  <h2> For the video Explanation of the Project <a href = 'https://drive.google.com/file/d/1PlYlgopGn3CSJcziYn-Jc9mnVFHHALYI/view?usp=sharing'>Click</a> here </h2>
</p>
