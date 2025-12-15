# MLOps Lifecycle with tools

This repo describes a visual representation of MLOps Lifecycle with MLOps Tools at each stage of lifecycle.

## High-level Architecture
<img width="1920" height="1080" alt="MLOps Lifecycle diagram" src="https://github.com/user-attachments/assets/b2db9898-587a-4d33-9a3a-d384bff4deee" />

## Lifecycle Stages & Tooling
### 1. Data Preparation
**Purpose:** This includes data collection, data ingestion, data validation and data pre-processing.
**Tools:** 
- Azure Data Factory/Airflow - Orchestrates and schedules data pipelines
- Pandas - Data cleaning and transformation
- Data Version Control (DVC) - Version control for datasets

### 2. Model Training
**Purpose:** This stage includes model development and training.
**Tools:**
- Tensorflow/Scikit-learn - Model development
- MLflow - Track parameters, metrics, artifacts

### 3. Model Validation
**Purpose:** This stage includes model performance evaluation for bias and robustness before deployment.
**Tools:**
- Scikit-learn metrics - Performance evaluation

### 4. Model Deployment
**Purpose:** This stage includes serving trained model for real-time or batch inference.
**Tools:**
- GitHub Actions/Azure DevOps - CI/CD pipelines
- Docker - Containerizes the model, code and dependencies
- MLflow Models - Model packaging and deployment

### 5. Monitoring
**Purpose:** This stage includes monitoring model performance and trigger retraining
**Tools:**
- Prometheus & Grafana - System and latency monitoring
- ELK stack - Logging and tracing

### 6. Retraining
**Purpose:** This stage includes collection of feedback, updating datasets and retraining models as required.
**Tools:**
- MLflow/Airflow pipelines - Retraining workflows
