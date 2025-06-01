# 📊 Capstone Project: Customer Purchase Prediction
### 🌟 Overview
Welcome to the Customer Purchase Prediction Capstone Project! This exciting machine learning pipeline predicts whether Indian customers will purchase a product based on Japanese customer data. It combines datasets from Japan and India, processes features, and trains three models—Logistic Regression, Random Forest, and Categorical Naive Bayes—to deliver powerful insights. Get ready to explore data-driven decision-making! 🚀
### ✨ Features

Data Sources: Combines JPN_DATA.xlsx (Japan) and IN_data.xlsx (India) for robust analysis.
Preprocessing:
Converts car maintenance dates in Indian data to AGE_CAR using a reference date (July 1, 2019).
Categorizes car age into buckets: <200, 200-360, 360-500, >500 days.
Encodes categorical variables like GENDER and car age categories.


Models: Trains and compares three algorithms:

📈 Logistic Regression

🌳 Random Forest Classifier

🧮 Categorical Naive Bayes


Prediction: Uses the best model (Logistic Regression) to predict purchases for Indian customers.
Output: Saves predictions to IND_data_with_predictions.xlsx and the model to model.pkl.

### 🛠️ Requirements
To embark on this journey, install these Python packages:
pip install numpy pandas seaborn matplotlib scikit-learn joblib

### 🚀 Usage

Prepare DataEnsure JPN_DATA.xlsx and IN_data.xlsx are in your working directory.
Run the Notebook  
Open capstone_project.ipynb in Jupyter Notebook or a similar environment.
Execute cells step-by-step to:
Load and clean Japanese and Indian datasets (no nulls found!).
Transform DT_MAINT into AGE_CAR for Indian data.
Categorize car ages and encode variables.
Merge datasets and train models.
Predict purchases for Indian customers.
Save results to IND_data_with_predictions.xlsx and the model to model.pkl.




Key Insights  
Logistic Regression achieved the highest accuracy (~68.73%) and R² score.
Predicted purchases for Indian customers: 66,967! 🌟
Check the console output for the number of predicted purchases.



### 📂 Project Structure

capstone_project.ipynb: The core script for data processing, modeling, and prediction.
JPN_DATA.xlsx: Japanese customer data with purchase history.
IN_data.xlsx: Indian customer data for prediction.
IND_data_with_predictions.xlsx: Output file with purchase predictions.
model.pkl: Saved Logistic Regression model for future use.

### 📊 Data Details

Features:
CURR_AGE: Current age of the customer
GENDER: Customer gender (encoded)
ANN_INCOME: Annual income of the customer
AGE_CAR: Age of the car in days
AGE_CAR_CATEGORY_*: Dummy variables for car age categories


Target:
PURCHASE: 1 if purchased, 0 otherwise (from Japanese data)


Output: PURCHASE_PREDICTION for Indian customers

### ⚠️ Notes

Data Quality: No null values detected in either dataset.
Model Warning: Logistic Regression may show a convergence warning; consider scaling data or increasing max_iter (see scikit-learn docs).
Performance: Logistic Regression outperformed others with ~68.73% accuracy.
Scalability: The model is saved as model.pkl for reuse—load it with joblib.load('model.pkl').

### 🤝 Contributing
We’d love your input! To contribute:

Fork this repository.
Create a branch for your feature or fix.
Submit a pull request with a clear description of your magic! ✨

### 📬 Contact
Questions or ideas? Open an issue on GitHub or reach out to the project maintainer. Let’s make predictions that shine! 🌟

#
Crafted with 💻 and a passion for machine learning!

