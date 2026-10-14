##  MindInsight  — Mental Health Score Prediction from Social Media Usage

FastAPI service that predicts an exploratory mental health score from social media usage, sleep, stress and lifestyle data. A scikit-learn pipeline (preprocessing + Random Forest) is served through a Pydantic-validated /predict endpoint and deployed on Render, with a simple web form on top.

## Link
Web app (frontend) ->	https://mindinsight-1.onrender.com


Hosted on Render's free tier, so the first load may take ~30–60 seconds while the service wakes up.


#Tech Stack
Tool	Purpose
Python,Pandas -> Data loading, cleaning, feature preparation
Scikit-learn ->	Preprocessing pipeline, model training, tuning, evaluation
Joblib ->	Saving the full pipeline (preprocessing + model) as one file
FastAPI ->	REST API with a /predict endpoint
Pydantic ->	Request validation (types, ranges, allowed categories)
Uvicorn ->	ASGI server that runs the API
HTML / CSS / JavaScript ->	Simple form frontend
Render -> Deployment of backend and frontend


