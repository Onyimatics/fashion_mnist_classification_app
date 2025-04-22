# fashion_mnist_classification_app
An end to end app to classify fashion mnist images using Streamlit interface and deployed as a docker container.

# Streamlit Application

A containerized Streamlit application running with Python 3.10.

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
3. Build the Docker image:
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