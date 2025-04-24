# fashion_mnist_classification_app
An end to end app to classify fashion mnist images using Streamlit interface and deployed as a docker container.

[//]: # (![Docker Build]&#40;https://img.shields.io/docker/build/onyimatics/fashion_mnist_classifier&#41;)
![Docker Build](https://img.shields.io/docker/cloud/build/onyimatics/fashion_mnist_classifier)
![Docker Build](https://img.shields.io/docker/automated/onyimatics/fashion_mnist_classifier)
![Docker Pulls](https://img.shields.io/docker/pulls/onyimatics/fashion_mnist_classifier)
![Docker Size](https://img.shields.io/docker/image-size/onyimatics/fashion_mnist_classifier)
![GitHub Repo watchers](https://img.shields.io/github/watchers/onyimatics/fashion_mnist_classification_app?style=social)
![GitHub Repo license](https://img.shields.io/github/license/onyimatics/fashion_mnist_classification_app)
![GitHub last commit](https://img.shields.io/github/last-commit/onyimatics/fashion_mnist_classification_app)
![GitHub contributors](https://img.shields.io/github/contributors/onyimatics/fashion_mnist_classification_app)
![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/onyimatics/fashion_mnist_classification_app)
![GitHub top language](https://img.shields.io/github/languages/top/onyimatics/fashion_mnist_classification_app)
![GitHub language count](https://img.shields.io/github/languages/count/onyimatics/fashion_mnist_classification_app)

# Streamlit Application

A containerized Streamlit application running with Python 3.10.

## Deployed Image on Docker Hub:
### [onyimatics/fashion_mnist_classifier](https://hub.docker.com/r/onyimatics/fashion_mnist_classifier)


## Requirements

- Docker
- Python 3.10
- pip

## Dependencies

- TensorFlow 2.16.2
- Streamlit 1.37.1
- NumPy 1.24.3

## Setup and Installation

### Local Setup
1. Clone the repository:
```bash
git clone <repository-url>
cd <repository-name>
```
2. Create and activate a virtual environment (recommended):
```bash
python -m venv venv
source venv/bin/activate  # On macOS
```

3. cd into app directory:
```bash
cd app
```
4. Install the required packages:
```bash
pip install -r requirements.txt
```

5. Start the application::
```bash
streamlit run main.py
```
6. Open your web browser and go to http://localhost:8501
7. Upload an image of a fashion item and click the "Classify" button to see the prediction.

### Docker Setup
1. Clone the repository:
```bash
git clone <repository-url>
cd <repository-name>
```

2. cd into app directory:
```bash
cd app
```
## Option A: Pull the pre-built image from Docker Hub:
```bash
docker pull onyimatics/fashion_mnist_classifier:v1.0
```
3. Then Run the Docker container:
```bash
docker run -p 80:80 onyimatics/fashion_mnist_classifier:v1.0
```
## Option B: Build the Docker image locally:
```bash
docker build -t fashion-mnist-app .
```
4. Run the Docker container:
```bash
docker run -p 80:80 fashion-mnist-app
```
5. Open your web browser and go to http://0.0.0.0:80
6. Upload an image of a fashion item and click the "Classify" button to see the prediction.
7. To stop the container, press `Ctrl+C` in the terminal where the container is running.
8. To remove the container, run:
```bash
docker rm <container-id>
```
9. To remove the image, run:
```bash
docker rmi fashion-mnist-app
```
10. To remove all stopped containers, run:
```bash
docker container prune
```
11. To remove all unused images, run:
```bash
docker image prune
```

Made with ❤️ by Onyinye Favour Ezike