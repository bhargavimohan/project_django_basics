# Use the latest Ubuntu LTS version as the base image
FROM ubuntu:latest

# Update package lists and install dependencies
RUN apt-get update && apt-get install -y \
    python3.10 \
    python3.10-dev \
    python3.10-distutils \
    curl \
    gnupg \
    && rm -rf /var/lib/apt/lists/*

# Install Node.js v18.x
RUN curl -fsSL https://deb.nodesource.com/setup_18.x | bash -
RUN apt-get install -y nodejs \
    && rm -rf /var/lib/apt/lists/*

# Optionally, you can install additional packages or perform any further setup here

# Set up a working directory
WORKDIR /app

# Set environment variables if needed

# Copy your application files into the container
# COPY . /app

# Specify any additional commands to run your application

# Example command to start your application
# CMD ["python3", "app.py"]
