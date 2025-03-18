Movie Rating Prediction Project

This project predicts the rating of Indian movies using machine learning models such as Decision Tree Regressor, Support Vector Regressor (SVR), and Gradient Boosting Regressor. It analyzes IMDb Indian movie data to extract insights and predict movie ratings based on multiple features.

📊 Project Features

Data Exploration & Visualization:

Identify the year with the best average rating.

Top 10 directors and actors with the most movies.

Visualize the relationship between movie duration and ratings.

Explore correlations between features using a heatmap and pair plots.

Feature Engineering:

Derived features: Genre Average Rating, Director Average Rating, and Actor Average Ratings.

Director's success rate based on the average rating of their movies.

Machine Learning Models:

Decision Tree Regressor

Support Vector Regressor (SVR)

Gradient Boosting Regressor

Model Evaluation:

Mean Squared Error (MSE)

Mean Absolute Error (MAE)

R² Score

Prediction:

Make predictions on sample movie data.

Compare model performances using scatter plots.

📁 Dataset

Ensure the dataset is downloaded from Kaggle and stored in Google Drive.

Download the dataset using kagglehub:

import kagglehub
path = kagglehub.dataset_download("adrianmcmahon/imdb-india-movies")
print("Dataset Path:", path)

Move the dataset to your Google Drive:

from google.colab import drive
import shutil

drive.mount('/content/drive')
shutil.move(path, '/content/drive/MyDrive/IMDb_Movies_India.csv')

🛠️ Setup Instructions

Clone this repository or download the script:

git clone <repository_url>
cd movie-rating-prediction

Install required libraries:

pip install pandas numpy seaborn matplotlib scikit-learn tensorflow keras

Ensure the dataset is available at the correct path:

Modify this line if needed:

df = pd.read_csv('/content/drive/MyDrive/IMDb Movies India.csv', encoding='ISO-8859-1')

Run the script:

python movie_rating_prediction.py

📈 Outputs

Year with the best average rating.

Top actors and directors by movie count.

Movie duration impact on rating (scatter plot).

Performance of Decision Tree, SVR, and Gradient Boosting models.

Predicted rating for trial data.

Sample Prediction Output:

Predicted Rating for trial data: 8.93

📊 Model Performance Comparison

The script evaluates three models and provides metrics:

Mean Squared Error (MSE)

Mean Absolute Error (MAE)

R² Score

🧹 Data Cleaning

Handles missing and duplicate values.

Converts data types for compatibility.

Adds derived features for better prediction.

📌 Notes

Ensure you have Python 3.8+ installed.

Customize the model or dataset paths as needed.

Modify the trial data in trail_data to test custom predictions.