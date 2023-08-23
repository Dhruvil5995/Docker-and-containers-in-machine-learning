# Docker-and-containers-in-machine-learning

## Machine Learning API using PyCaret, FastAPI, and Docker

## Overview

This repository showcases the creation of a robust machine learning API using the powerful PyCaret library for streamlined model training, the versatile FastAPI framework for building API endpoints, and Docker for seamless containerization. By combining these technologies, the project illustrates a comprehensive workflow for developing, deploying, and managing machine learning models as accessible APIs.

## Project Structure

The project is organized into the following key files and directories:

- `create container for an API.ipynb`: A Python script that initializes a PyCaret experiment, trains a machine learning model on a dataset, and saves the trained model for future use.
- `my_first_api.py`: A FastAPI script that defines the API endpoints, enabling users to submit input data for predictions using the trained model.
- `Dockerfile`: Contains instructions for building a Docker container that encapsulates the API and its dependencies.
- `requirements.txt`: Lists the required dependencies and their versions.
- `README.md`: This documentation file, providing an overview, instructions, and project details.

## Usage Instructions

1. **Clone the Repository**: Begin by cloning the repository to your local environment using the following command:

   (https://github.com/Dhruvil5995/Docker-and-containers-in-machine-learning.git)

#### Training the Model: To train the machine learning model and save it for future use, execute the following command:

see the Create container for an API.ipynb File
#### Running the FastAPI App: Navigate to the api directory and launch the FastAPI app using Uvicorn:

uvicorn my_first_api:app --host 127.0.0.1 --port 8000

#### Building and Running the Docker Container: In the project root directory, build and run the Docker container:

docker build -t my_ml_api .
docker run -p 8000:8000 my_ml_api
#### Accessing the API: Open a web browser or use tools like curl or Postman to make POST requests to http://127.0.0.1:8000/predict with the necessary input parameters.

### Dependencies
Python 3.8 or higher
PyCaret 2.3.5
FastAPI 0.68.0
Uvicorn 0.15.0
Pandas 1.3.3
### License
This project is licensed under the MIT License. For more details, refer to the LICENSE file.

### Contributing
Contributions, issues, and feedback are welcome! Feel free to submit issues or open pull requests.
