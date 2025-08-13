# MLOps Pipeline for Network Security System

## Overview
This repository contains a production-ready MLOps pipeline designed for network security. The system focuses on detecting and classifying malicious URLs using machine learning, ensuring safe network traffic. The pipeline includes data ingestion, preprocessing, model training, deployment, and monitoring.

---

## Technology Stack
- **Programming Language:** Python  
- **Machine Learning Libraries:** scikit-learn, TensorFlow  
- **Data Storage:** MongoDB Atlas  
- **Cloud Infrastructure:** AWS (EC2, S3, ECR)  
- **Containerization:** Docker  
- **CI/CD Tools:** GitHub Actions  
- **Model Monitoring:** MLflow  
- **Web Framework:** FastAPI  
- **Version Control:** Git/GitHub  

---

## Features
- **Data Ingestion & ETL Pipelines:** Automated extraction, transformation, and loading of network traffic data.  
- **Model Training & Evaluation:** Train ML models to classify URLs as malicious or benign.  
- **Model Deployment:** Dockerized deployment on AWS EC2.  
- **CI/CD Automation:** GitHub Actions workflows for continuous integration and deployment.  
- **Model Monitoring:** Track model performance and versions using MLflow.  
- **API Interface:** RESTful API for predictions using FastAPI.  

---

## Repository Structure
├── .github/ # GitHub Actions workflows
├── networksecurity/ # Core application code
│ ├── app.py # FastAPI app
│ ├── main.py # Model inference logic
│ ├── push_data.py # Data ingestion script
│ └── utils.py # Utility functions
├── data/ # Sample data files
├── models/ # Trained model artifacts
├── requirements.txt # Python dependencies
├── Dockerfile # Docker configuration
├── setup.py # Package setup
├── test_mongodb.py # MongoDB connection tests
└── README.md # Project documentation

yaml
Copy
Edit

---

## Setup & Installation

### Prerequisites
- Python 3.8+  
- Docker  
- AWS account (EC2, S3, ECR)  
- MongoDB Atlas account  

### Installation
1. Clone the repository:
```bash
git clone https://github.com/prathmkapde17/MLOps-Pipeline-for-Network-Security-System.git
cd MLOps-Pipeline-for-Network-Security-System
Set up a virtual environment:

bash
Copy
Edit
python3 -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
Install dependencies:

bash
Copy
Edit
pip install -r requirements.txt
Configure AWS credentials (using AWS CLI or environment variables).

Build Docker image:

bash
Copy
Edit
docker build -t network-security-api .
Run the application:

bash
Copy
Edit
uvicorn networksecurity.app:app --reload
Deployment
Deploy the application to AWS EC2 and manage models using ECR. The repository includes Docker support for smooth deployment.

CI/CD
Automated workflows using GitHub Actions handle building, testing, and deploying updates.

Model Monitoring
Use MLflow for tracking experiments, logging metrics, and managing model versions.

License
This project is licensed under the MIT License. See the LICENSE file for details.

Contact
For questions or contributions, contact Prathmesh Kapde.
