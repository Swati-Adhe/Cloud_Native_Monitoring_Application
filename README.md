# Cloud Native Monitoring Application

This project is a simple Cloud Native Monitoring Application built using Flask and `psutil`. The application monitors CPU and memory usage, displaying a warning message when the usage exceeds 80%.

## Prerequisites

- Python 3.9+
- Docker

## Setup and Installation

### 1. Clone the Repository

```bash
git clone https://github.com/Swati-Adhe/Cloud_Native_Monitoring_Application.git
cd Cloud_Native_Monitoring_Application
```
## Running the Application Locally

### 2. Install Dependencies

If you are running the application locally without Docker, install the required Python packages:
```bash
pip install -r requirements.txt
```

### Run the Application
```bash
python app.py
```
The application will be accessible at http://127.0.0.1:5000/.

## Dockerization
### 1. Build the Docker Image
```bash
docker build -t cloud-native-monitoring-app .
```

### 2. Run the Docker Container
```bash
docker run -d -p 5000:5000 cloud-native-monitoring-app
```
This will start the Flask server in a Docker container on localhost:5000. Navigate to http://localhost:5000/ on your browser to access the application.

## Application Details

- **CPU Metric**: Displays the current CPU usage percentage.
- **Memory Metric**: Displays the current memory usage percentage.
- **Alert Message**: Displays an alert message when CPU or memory usage exceeds 80%.

## Future Work

This project is ongoing and will continue to evolve. Future enhancements include:

- **Create ECR Repository**: Implementing an ECR repository using Python Boto3 and pushing Docker images to ECR.
- **Learn Kubernetes**: Acquiring knowledge in Kubernetes and setting up an EKS cluster and NodeGroups.
- **Kubernetes Deployments and Services**: Developing Kubernetes Deployments and Services using Python.

Stay tuned for updates!

