# US-Visa-Approval-System

A machine learning-based system for predicting US visa approval outcomes. This project uses various machine learning models, with the K-Nearest Neighbors (KNN) model achieving a remarkable accuracy of 96.6%. It is built with FastAPI for a scalable backend and MongoDB for database storage.

## 🚀 Features
- High Accuracy Predictions: Predict visa approval status using the KNN model.
- Scalable Backend: Built with FastAPI for speed and efficiency.
- Database Integration: Uses MongoDB for storing visa application data.
- Machine Learning Pipeline: Experimented with multiple models to achieve optimal performance.

## 🛠️ Installation

### Prerequisites
Ensure you have the following installed:
- Python 3.8 or higher
- MongoDB
- FastAPI

## Steps

1. Clone the Repository
```
git clone https://github.com/princ0301/US-Visa-Approval-System.git  
cd US-Visa-Approval-System
```

2. Install Dependencies
```
pip install -r requirements.txt
```

3. Set Up Environment Variables
Create a .env file in the project root directory and add the following:
```
MONGODB_URI="your_mongodb_connection_string"  
DATABASE_NAME="visa_db"  
COLLECTION_NAME="visa_applications"  
```

4. Run the Application
Start the FastAPI server:
```
uvicorn app.main:app --reload  
```

## 💡 Usage
- Data Ingestion: Insert visa application data into the MongoDB database.
- Model Inference: Use the /predict API endpoint to get approval predictions.

## 🧪 Machine Learning Models
### Experimented models include:

- Logistic Regression
- Decision Trees
- Random Forest
- Support Vector Machines (SVM)
- K-Nearest Neighbors (KNN) (final model with 96.6% accuracy)

## 🔗 API Endpoints
- GET /healthcheck
 Check API health status.

- POST /predict
  Predict visa approval status by submitting application details.

- GET /applications
  Retrieve visa applications stored in the database.

## 🤖 Technologies Used

- FastAPI: Backend API development
- MongoDB: Database for storing application data
- scikit-learn: Machine learning pipeline
- pandas & numpy: Data preprocessing and analysis
