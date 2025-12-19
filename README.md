# housing-price-ml-gcp--
End-to-end machine learning project that predicts housing prices using scikit-learn, trained in Google Colab and designed for deployment on Google Cloud Vertex AI.
#  Housing Price Prediction (Machine Learning)

This project is an end-to-end machine learning solution for predicting housing prices using Python and scikit-learn.  
The model is trained in **Google Colab** and designed to be **cloud-ready for Google Cloud Vertex AI** deployment.

---

#Project Overview

The goal of this project is to predict house prices based on multiple features such as:
- Area
- Number of bedrooms and bathrooms
- Parking availability
- Furnishing status
- Other housing attributes

The project demonstrates a complete ML workflow:
- Data loading and preprocessing
- Feature encoding
- Model training and evaluation
- Model persistence
- Cloud storage integration

---

# Technologies Used

- Python
- pandas
- numpy
- scikit-learn
- joblib
- Google Colab
- Google Cloud Storage (GCS)

---

# Dataset

The dataset contains both numerical and categorical features related to housing properties.

**Target variable:**  
- `price` — the house price to be predicted

Categorical variables are encoded using one-hot encoding before training.

---

# Model

- Algorithm: **RandomForestRegressor**
- Evaluation metric: **RMSE (Root Mean Squared Error)**

The trained model is saved as:


---

model.joblib

# Model Performance

The model achieves a reasonable RMSE, demonstrating effective learning from the dataset and suitability for regression tasks involving real-world housing data.

---

# Cloud Integration

The trained model is uploaded to **Google Cloud Storage**, making it ready for:
- Vertex AI model registration
- Online or batch prediction deployment

This project follows best practices for cloud-based ML workflows.

---

# How to Run the Project

1. Open the notebook in **Google Colab**
2. Upload the dataset (`Housing.csv`)
3. Install dependencies:
   ```bash
   pip install -r requirements.txt

4,Run all cells to:

Train the model

Evaluate performance

Save and upload the model

### Future Improvements

Hyperparameter tuning

Experimenting with Gradient Boosting / XGBoost

Deployment to a Vertex AI Endpoint

Building a REST API for predictions
