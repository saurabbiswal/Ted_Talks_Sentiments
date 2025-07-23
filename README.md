TED Talk View Prediction

This project aims to build an end-to-end regression model that predicts the number of views a TED Talk is likely to get, using metadata and transcript features. It demonstrates core MLOps principles including reproducibility, scalability, and automation.

⸻

🚀 Objective

To predict the exact number of views a TED Talk will receive, based on its:
	•	Transcript text
	•	Title and tags
	•	Speaker details
	•	Duration and publication date

This will help:
	•	Understand what content, topics, or speaker traits drive more viewership
	•	Explore patterns in TED Talk popularity
	•	Showcase full-cycle ML engineering skills (data, modeling, deployment, monitoring)

⸻

🔧 Project Scope

The project will cover:
	•	📥 Data Ingestion
	•	✅ Data Validation & Cleaning
	•	✨ Feature Engineering (TF-IDF, stopword counts, etc.)
	•	🤖 Model Training using ML models:
	•	Logistic Regression
	•	Random Forest
	•	XGBoost
	•	Naive Bayes (for baseline)
	•	📊 Evaluation using regression metrics (R2, RMSE)
	•	🧪 MLflow Tracking (local or remote via EC2)
	•	📦 Model Packaging via Flask API
	•	☁️ Deployment on AWS EC2
	•	🔁 CI/CD Integration (GitHub Actions + EC2)

⸻

📁 Folder Structure

TED_Talk_Sentiment/
│
├── data/                   # Raw and processed data
├── notebooks/              # Jupyter notebooks (EDA, modeling)
├── src/                    # Source code (data, training, etc.)
│   ├── data_ingestion.py
│   ├── feature_engineering.py
│   ├── train.py
│   └── model_evaluation.py
│
├── app/                    # Flask API code for model serving
├── mlruns/                 # MLflow run tracking (if local)
├── requirements.txt
├── .gitignore
├── README.md
└── config/                 # Config files (MLflow URI, model params, etc.)


⸻

🔍 Notes
	•	✅ This is a regression problem, not classification (i.e., we predict a continuous value — view count).
	•	🧠 We will tune and compare multiple models using MLflow.
	•	🌐 EC2 will host both the MLflow server and Flask app in production.

⸻

📌 To Do
	•	Git repo initialized
	•	Data exploration in notebook
	•	Baseline model implementation
	•	MLflow integration (local → EC2 param switch)
	•	Flask API setup
	•	CI/CD pipeline configuration

⸻

👨‍💻 Author

Saurabh Biswal
Exploring end-to-end MLOps with real-world TED data