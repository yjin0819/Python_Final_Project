# Movie Critic Rating Prediction

This repository contains a complete machine learning workflow for predicting movie critic ratings. The project aims to develop predictive models that can estimate movie critic scores based on various features such as runtime, genre, audience feedback, and more. This project is the MLDS 422 final project.

## Project Structure

The repository includes:

- **README file** (this document): Provides an overview of the project, its purpose, and the contents of the repository.
- **Code**: Jupyter Notebook(s)  containing all the steps for data gathering, cleaning, exploratory data analysis, feature engineering, and model development.
- **Data**: The data used for the project, stored in CSV files(data.csv.zip). The dataset was sourced from the NU MLDS 2024 server.
- **Requirements**: A requirements.yml file listing the required Python packages to replicate the environment used in the project.

## Workflow Summary
The main components of this project are organized into different parts in the code:
1. **Data Gathering and Scope**: Connected to the NU MLDS 2024 server using psycopg to gather movie data and explored the data to create a predictive model for movie critic ratings.
2. **Data Cleaning and Exploratory Data Analysis (EDA)**: Loading the dataset, handling missing values, analyzed the movie dataset, visualized yearly movie releases, identified erroneous values, and performed exploratory data analysis to gain insights into the data. Specific analyses included identifying top-rated movies by both critics and audiences, defining "popular" movies, and investigating movie ratings trends.
3. **Feature Engineering**: Created new features such as a "kid-friendly" indicator and dummy variables for genres, along with other derived features. Split the data into training and testing sets based on release years, with pre-2010 movies for training and movies released in 2010 and later for testing.
4. **Modeling**: Developed multiple linear regression models using different feature combinations to predict critic ratings. Evaluated these models based on metrics such as R-squared, Mean Absolute Error (MAE), and Root Mean Squared Error (RMSE). Iteratively improved model performance by adding, removing, or combining features. Also provided insights from models.

## Usage

To replicate this project, simply clone this repository,set up the required Python environment listed in the requirements.yml file and also download the data.csv.zip, and open the Jupyter notebooks to walk through the steps taken in each phase of the project.

Make sure to also set up a PostgreSQL connection to access the dataset if you want to retrieve fresh data from the original database.


## Results and Analysis

- Six different linear regression models were fitted, with iterative improvements through feature selection and feature engineering.
- Key insights were derived from model performances, and recommendations were made on how to further improve prediction accuracy, such as experimenting with more advanced modeling techniques (e.g., Random Forest).

## License

This project is not licensed for commercial use.

## Notes

- The credential used to connect to the database for getting the original data has been removed from the Code
- This repository was made private for the duration of grading, but may be made public afterward to serve as a portfolio project.
