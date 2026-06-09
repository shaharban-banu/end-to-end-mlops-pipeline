# End-to-End MLOps Pipeline with FastAPI, Docker, AWS ECR, SageMaker and GitHub Actions

Project Overview :

This project demonstrates an end-to-end MLOps pipeline for deploying a Machine Learning model using AWS cloud services and CI/CD automation.

The pipeline trains an Iris flower classification model, packages it inside a Docker container with a FastAPI inference service, pushes the image to Amazon ECR, and automatically deploys it to Amazon SageMaker using GitHub Actions.

Architecture :

Developer
    │
    ▼
GitHub Repository
    │
    ▼
GitHub Actions (CI/CD)
    │
    ├── Build Docker Image
    ├── Push Image to Amazon ECR
    └── Update SageMaker Endpoint
            │
            ▼
      Amazon SageMaker
            │
            ▼
      Live Inference Endpoint

Tech Stack :

Machine Learning
Python
Scikit-learn
NumPy
API Development
FastAPI
Uvicorn
Containerization
Docker
Cloud Services
AWS SageMaker
AWS ECR
AWS IAM
AWS CloudWatch
DevOps & CI/CD
GitHub Actions
Git
GitHub

Running the Project Locally :

Install Dependencies
pip install -r requirements.txt
Train Model
python train.py
Run FastAPI
uvicorn app:app --host 0.0.0.0 --port 8080
Open Swagger UI
http://localhost:8080/docs
