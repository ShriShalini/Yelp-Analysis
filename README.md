# Yelp-Analysis

Yelp publishes crowd sourced reviews about businesses based on activity on their site and app.
The Yelp Dataset includes information about:
 - User
 - Review
 - Business
 - Tips
 - Checkin

This repository leverages yelp dataset to answer the question **"Would a business survive after the year#?"**
The year# can be values within the bounds of the dataset, but in this repository the year 2020 is considered.

This project is also containerized with Docker and the image is store in DockerHub registry. 
One could pull the image into their machine and run using the following steps.

Prerequisites: Docker Desktop Application (Downloaded here: https://www.docker.com/products/docker-desktop/), DockerHub account (https://hub.docker.com/)

**Steps to the run:**
- Open the Docker Desktop application (very important)
- Open the terminal
- Type **"docker"** (This should not throw any error like "docker cannot be found"). This should show the docker help documentation.
- Type **"docker login"**
- Enter the username and password of your DockerHub account when prompted. 
- Type **"docker run -p 8888:8888 -it shrishalinisekar/yelp:latest"**
- Three URLs would be given with which the file can be accessed. Try all three, choose the one that opens a JupyterLab.
- Once the JupyterLab is open, open the Yelp_data_analysis.ipynb
- Click on Run->Run All Cells to run all cells to see the analysis.
