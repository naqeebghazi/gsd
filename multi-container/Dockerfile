# Base image
FROM python:alpine

# Add app code to /code inside container image
ADD . /code

# Set working directory for subsequent commands
WORKDIR /code

# Install dependencies
RUN pip install -r requirements.txt
RUN curl -fsSL https://get.docker.com | sh

# Command to run when container starts
ENTRYPOINT ["python", "app.py"]