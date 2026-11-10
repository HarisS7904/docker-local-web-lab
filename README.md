# Overview

The goal is to learn how to build a Docker image, run a Python web server
inside a container and access it through a web browser.

# Technologies Used

- Docker
- Python 3
- Ubuntu (WSL2)
- Git and GitHub

# Project Structure
```text
docker-local-web-lab/
├── app.py
├── Dockerfile
├── .dockerignore
├── README.md
└── troubleshooting.md
```

# How to Run

1. Build the Docker Image
```bash
docker build -t docker-local-web-lab .
```
This builds a Docker image using the instructions in the `Dockerfile`.

2. Run the Container
```bash
docker run --rm -p 8080:8000 docker-local-web-lab
```
This starts the Python web server inside a Docker container.

3. Access the Web Server
Open browser and visit:
```text
http://localhost:8000
```

4. Stop the Container
Press `Ctrl+C` in the terminal running the container.

# Topics

- The difference between Docker images and containers.
- How to create a Dockerfile.
- How to build a Docker image.
- How to run a container.
- How Docker port mapping works.
- Why `.dockerignore` is useful.

# Troubleshooting

All issues encountered during practices will be documented in `troubleshooting.md`
