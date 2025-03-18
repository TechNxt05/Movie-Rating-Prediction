# Movie Rating Prediction Project

This project predicts the rating of Indian movies using machine learning models such as Decision Tree Regressor, Support Vector Regressor (SVR), and Gradient Boosting Regressor. It analyzes IMDb Indian movie data to extract insights and predict movie ratings based on multiple features.

## 📊 Project Features

_Data Exploration & Visualization:_

Identify the year with the best average rating.

Top 10 directors and actors with the most movies.

Visualize the relationship between movie duration and ratings.

Explore correlations between features using a heatmap and pair plots.

## Feature Engineering:

Derived features: Genre Average Rating, Director Average Rating, and Actor Average Ratings.

Director's success rate based on the average rating of their movies.

_Machine Learning Models:_

* Decision Tree Regressor

* Support Vector Regressor (SVR)

* Gradient Boosting Regressor

_Model Evaluation:_

* Mean Squared Error (MSE)

* Mean Absolute Error (MAE)

* R² Score

_Prediction:_

Make predictions on sample movie data.

Compare model performances using scatter plots.

## 📁 Dataset

Ensure the dataset is downloaded from Kaggle and stored in Google Drive.

* _Download the dataset using kagglehub:_

'''bash
import kagglehub
path = kagglehub.dataset_download("adrianmcmahon/imdb-india-movies")
print("Dataset Path:", path)
'''

* _Move the dataset to your Google Drive:_

'''bash
from google.colab import drive
import shutil

drive.mount('/content/drive')
shutil.move(path, '/content/drive/MyDrive/IMDb_Movies_India.csv')
'''

## 🛠️ Setup Instructions

* _Clone this repository or download the script:_

'''bash
git clone <repository_url>
cd movie-rating-prediction
'''

* _Install required libraries:_

'''bash
pip install pandas numpy seaborn matplotlib scikit-learn tensorflow keras
'''

* _Ensure the dataset is available at the correct path:_

_Modify this line if needed:_

'''bash
df = pd.read_csv('/content/drive/MyDrive/IMDb Movies India.csv', encoding='ISO-8859-1')
'''

_Run the script:_

'''bash
python movie_rating_prediction.py
'''

## 📈 Outputs

* Year with the best average rating.

* Top actors and directors by movie count.

* Movie duration impact on rating (scatter plot).

* Performance of Decision Tree, SVR, and Gradient Boosting models.

* Predicted rating for trial data.

_Sample Prediction Output:_

'''bash
Predicted Rating for trial data: 8.32
'''

## 📊 Model Performance Comparison

_The script evaluates three models and provides metrics:_

* Mean Squared Error (MSE)

* Mean Absolute Error (MAE)

R² Score

## 🧹 Data Cleaning

* Handles missing and duplicate values.

* Converts data types for compatibility.

* Adds derived features for better prediction.

## 📌 Notes

* Ensure you have Python 3.8+ installed.

* Customize the model or dataset paths as needed.

* Modify the trial data in trail_data to test custom predictions.
