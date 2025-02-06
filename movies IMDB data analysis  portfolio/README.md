# Movies & Directors Dataset Analysis

## Project Overview

This project analyzes a **Movies & Directors Dataset** using **SQL (SQLite)** and **Python (pandas, NumPy, Matplotlib)** to extract valuable insights about movie budgets, revenues, popularity, and director performances. The analysis focuses on statistical exploration, revenue trends, and director-based comparisons to uncover patterns and trends in the film industry.

## Technologies Used

- **Programming Language**: Python
- **Libraries**: pandas, numpy, matplotlib, sqlite3
- **visualization tool**: powerBI
- **Database**: SQLite (**movies_directors_dataset.sqlite**)
- **Development Environment**: Jupyter Notebook 

## Dataset Information

### Movies Table Columns:
- **id**: Unique movie identifier
- **original_title**: Original name of the movie
- **budget**: Movie production budget
- **popularity**: Popularity score of the movie
- **release_date**: Release date of the movie
- **revenue**: Total revenue generated
- **title**: Movie title
- **vote_average**: Average rating given by users
- **vote_count**: Number of votes received
- **overview**: Brief summary of the movie
- **tagline**: Promotional tagline of the movie
- **uid**: Unique identifier
- **director_id**: ID of the movie's director

### Directors Table Columns:
- **name**: Director's name
- **id**: Unique director identifier
- **gender**: Gender of the director (0-Male, 1-Female, 2-Male)
- **uid**: Unique identifier
- **department**: Department of the director

## Steps Performed

### 1. Importing Necessary Libraries
- Imported numpy for numerical computations
- Imported pandas for data manipulation
- Imported matplotlib.pyplot for data visualization
- Imported sqlite3 for database connection

### 2. Database Connection
- Established connection to SQLite database (**movies_directors_dataset.sqlite**)
- Created a cursor object to execute SQL queries

### 3. Data Exploration
- Retrieved all records from the movies and directors tables
- Created Pandas DataFrames for easy manipulation
- Displayed dataset structure using `info()`, `describe()`, and `head()`
- Checked unique values, missing data, and performed basic statistical analysis

### 4. Exploratory Data Analysis (EDA)
- **Budget Analysis**: Identified top 10 highest-budget movies
- **Revenue Analysis**: Extracted top 10 highest-revenue movies
- **Popularity Analysis**: Found the top 3 most popular movies
- **Voting Analysis**: Analyzed top-voted movies post-2005

**Director Analysis**:
- Counted movies directed by each director
- Identified the highest-grossing directors
- Extracted movies directed by specific directors (e.g., Steven Spielberg)
- Counted the number of female directors in the dataset

**JOIN Operations**:
- Combined movies and directors data for a comprehensive dataset

**CSV Export**:
- Converted final dataset into a CSV file for further analysis

### Data Visualization
- I have created dashboard using powerBI for the project visual and uploded that file inside the 02_scripts whicha have total 3 pages and also i have extracted year from released_date & dashboard images 03_output/a_visualizations(dashboard_image) directory of the portfolio folder

### 5. Key Insights

#### Insight 1: Director with the Most Movies
- **Finding**: Steven Spielberg directed the most movies in the dataset.
- **Interpretation**: Spielberg's extensive filmography reflects his lasting influence and creativity in the industry.

#### Insight 2: Most Bankable Director
- **Finding**: Steven Spielberg also had the highest total movie budget.
- **Interpretation**: His ability to secure high-budget projects highlights his credibility and industry stature.

#### Insight 3: Top 5 Directors by Total Movie Budget
- **Finding**: The leading directors in total movie budget include Steven Spielberg, Michael Bay, Peter Jackson, Ridley Scott, and Bryan Singer.
- **Interpretation**: These directors have consistently worked on large-scale projects.

#### Insight 4: Most Expensive Movie per Director
- **Finding**: Each director has at least one significantly high-budget film.
- **Interpretation**: This indicates varying production investments among different directors.

#### Insight 5: Most Popular Movies
- **Finding**: The top 5 most popular movies include Minions, Interstellar, Deadpool, Guardians of the Galaxy, and Mad Max: Fury Road.
- **Interpretation**: These movies have achieved widespread audience engagement and cultural impact.

#### Insight 6: Movies with the Highest Vote Counts
- **Finding**: Inception, The Dark Knight, and Avatar received the most votes.
- **Interpretation**: These films maintain high viewer engagement and critical acclaim.

#### Insight 7: Directors with the Highest Average Vote Count
- **Finding**: Directors like Tim Miller, Christopher Nolan, and Joss Whedon have the highest average votes per movie.
- **Interpretation**: Their movies consistently attract audience approval and engagement.

## Folder Structure
## 01_data
- **movies_directors_dataset.sqlite** :S QLite database containing movies and directors tables.
- **movies-directors_cleaned_dataset.csv**: Preprocessed dataset combining movie and director details.

## 02_scripts
- **a_common_imports.ipynb**: Commonly used imports o library like numpy ,pandas,matplotlib and othe libraries
- **b_database_connection.ipynb** :Script to connect to the SQLite database.
- **c_data_exploration.ipynb**: Basic exploratory data analysis (EDA).
- **d_exploratory_data_analysis(eda).ipynb**:Advanced EDA with visualizations.
- **e_insights_code.ipynb**: Code to extract key insights from the data.
- **movies IMDB data analysis visualization using powerBi.pbix**:this contains the powerBI dashboards created by powerBI

## 03_output
### a_visualizations(dashboard_image)
- **movies IMDB data analysis Page1.png**:contains project dashboard page 1
- **movies IMDB data analysis Page2.png**:contains project dashboard page 2
- **movies IMDB data analysis Page3.png**:contains project dashboard page 3
### b_report
- **insights.md**: Summary of key findings and insights.

Other Files:
                                                                                      
**README.md**
Project overview and methodology.

**requirements.txt**
List of required dependencies.

## Conclusion
This project successfully explores the Movies & Directors dataset to uncover meaningful insights about movie budgets, revenues, popularity, and director success rates. The findings can assist film industry professionals in making data-driven decisions regarding movie production and director collaborations.
