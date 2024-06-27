# Counter Service

This repository contains the code for the Counter Service, which is built using Python Flask. It also includes a Dockerfile for containerizing the application.

## Repository Structure

- `app.py`: Main application file containing the Flask code.
- `Dockerfile`: File used to build the Docker image for the Counter Service.

## Building and Pushing the Docker Image

The Docker image for this application is built using the infrastructure defined in the `devops-infra` repository. Below are the steps to build and push the image to AWS ECR.


### Build the Docker Image

1. Navigate to the `devops-infra` repository 
2. Set the following secrets:
    - AWS_ACCESS_KEY_ID
    - AWS_SECRET_ACCESS_KEY
    - COUNTER_SERVICE_REPO_PAT
3. Run the workflow named "Build & Push Docker Image"