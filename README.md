# 🎓 Student Performance Prediction (MLOps Project)

An end-to-end **Machine Learning Operations (MLOps)** project focused on predicting student academic performance, specifically **Math Scores**, using multiple regression algorithms and production-ready engineering practices.

This project demonstrates the complete ML lifecycle including:

- Data Ingestion
- Data Transformation
- Model Training
- Model Evaluation
- Pipeline Creation
- Dockerization
- Deployment-ready architecture

---

# 📌 Problem Statement

The goal of this project is to predict a student's **Math Score** based on several factors such as:

- Gender
- Race/Ethnicity
- Parental Level of Education
- Lunch Type
- Test Preparation Course
- Reading Score
- Writing Score

The project follows a modular and scalable MLOps workflow suitable for real-world deployment scenarios.

---

# 🚀 Features

✅ Modular project structure  
✅ End-to-end ML pipeline  
✅ Data preprocessing pipeline  
✅ Hyperparameter tuning  
✅ Multiple ML models comparison  
✅ Logging and exception handling  
✅ Docker support  
✅ Production-ready code organization  
✅ Flask/Streamlit application support  

---

# 🧠 Machine Learning Workflow

## 1️⃣ Data Ingestion
- Reads dataset from source
- Splits into train/test datasets
- Stores artifacts for pipeline usage

## 2️⃣ Data Transformation
- Handles categorical encoding
- Feature scaling
- Preprocessing pipeline creation using Scikit-Learn

## 3️⃣ Model Training
Models trained and evaluated:

- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor
- Gradient Boosting Regressor
- AdaBoost Regressor
- XGBoost Regressor
- CatBoost Regressor

## 4️⃣ Model Evaluation
Evaluation Metric:

- **R² Score**

### 🏆 Best Performing Model

| Model | R² Score |
|------|------|
| Linear Regression | **0.8804** |

---

# 📊 Exploratory Data Analysis (EDA)

Key insights obtained from the dataset:

### 📌 Test Preparation Helps
Students who completed the test preparation course generally performed better in exams.

### 📌 Reading & Writing Scores Matter
Reading and writing scores show strong positive correlation with math scores.

### 📌 Socio-Economic Factors
Lunch type and parental education level influence student performance.

### 📌 Linear Relationship
The dataset exhibited strong linear relationships, making Linear Regression highly effective.

---

# 🏗️ Project Structure

```plaintext
student-performance-mlops/
│
├── artifacts/                     # Saved models & preprocessors
│   ├── model.pkl
│   └── preprocessor.pkl
│
├── notebook/                      # EDA & experimentation notebooks
│
├── src/
│   ├── components/
│   │   ├── data_ingestion.py
│   │   ├── data_transformation.py
│   │   └── model_trainer.py
│   │
│   ├── pipeline/
│   │   ├── predict_pipeline.py
│   │   └── train_pipeline.py
│   │
│   ├── logger.py
│   ├── exception.py
│   └── utils.py
│
├── templates/                     # HTML templates (if Flask app)
├── static/                        # Static assets
│
├── app.py                         # Main application
├── requirements.txt               # Dependencies
├── setup.py                       # Packaging setup
├── Dockerfile                     # Docker configuration
├── README.md
│
└── .gitignore
```

---

# ⚙️ Installation & Setup

## 1️⃣ Clone the Repository

```bash
git clone https://github.com/MedisettiVinay0519/ML-Student-Performance-Pipeline 
cd student-performance-mlops
```

---

## 2️⃣ Create Virtual Environment (Optional but Recommended)

### Windows

```bash
python -m venv venv
venv\Scripts\activate
```

### Linux/Mac

```bash
python3 -m venv venv
source venv/bin/activate
```

---

## 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

---

# ▶️ Running the Project

## Run Training Pipeline

```bash
python src/components/data_ingestion.py
```

---

## Run the Application

```bash
python app.py
```

Application runs on:

```plaintext
http://localhost:8080
```

---

# 🐳 Dockerization

The project is fully containerized using Docker.

## Build Docker Image

```bash
docker build -t student-performance-app .
```

---

## Run Docker Container

```bash
docker run -p 8080:8080 student-performance-app
```

Application URL:

```plaintext
http://localhost:8080
```

---

# 📦 Tech Stack

## Programming Language
- Python

## Machine Learning
- Scikit-Learn
- XGBoost
- CatBoost

## Data Processing
- Pandas
- NumPy

## MLOps & Deployment
- Docker
- Logging
- Exception Handling

## Web Framework
- Flask / Streamlit

---

# 📈 Model Evaluation Results

| Model | Status |
|------|------|
| Linear Regression | Best Model |
| Random Forest | Evaluated |
| Decision Tree | Evaluated |
| Gradient Boosting | Evaluated |
| AdaBoost | Evaluated |
| XGBoost | Evaluated |
| CatBoost | Evaluated |

---

# 🔥 Future Improvements

- CI/CD Pipeline Integration
- Kubernetes Deployment
- MLflow Experiment Tracking
- AWS/GCP Deployment
- Monitoring & Logging Dashboard
- Model Drift Detection
- API Deployment with FastAPI

---

# 🛡️ Exception Handling & Logging

Custom logging and exception handling are implemented for:

- Easier debugging
- Better monitoring
- Production-grade reliability

---

# 📚 Learning Outcomes

Through this project, the following concepts were implemented and practiced:

- End-to-End ML Pipeline
- Production-level ML Coding Structure
- Feature Engineering
- Hyperparameter Tuning
- Dockerization
- MLOps Best Practices
- Model Serialization
- Pipeline Automation

---

