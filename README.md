# Docker Basics – Task 9

## Objective
To understand Docker fundamentals by containerizing a simple application.

## Tools Used
- Docker
- Python
- Flask

## Project Description
This project demonstrates basic Docker usage by running a simple Flask application inside a Docker container.

---

## Steps Performed

### 1. Docker Installation
- Installed Docker on the system
- Verified installation using:
  - docker --version
  - docker info

### 2. Application Creation
- Created a simple Flask application (`app.py`)
- Added required dependency in `requirements.txt`

### 3. Dockerfile Creation
- Used Python base image
- Set working directory
- Installed dependencies
- Copied application code
- Exposed port 5000
- Defined container run command

### 4. Docker Image Build
Command used:
# Check Docker installation
docker --version
docker info

# Build Docker image
docker build -t docker-task9-app .

# List Docker images
docker images

# Run Docker container
docker run -d -p 5000:5000 --name task9-container docker-task9-app

# List running containers
docker ps

# View container logs
docker logs task9-container

# Stop running container
docker stop task9-container

# Remove container
docker rm task9-container

# Remove Docker image
docker rmi docker-task9-app

---

## Output
The Flask application runs successfully inside a Docker container and displays:
Hello from Docker!

---

## Author
Devipriya 
