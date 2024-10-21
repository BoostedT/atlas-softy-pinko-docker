# Use the latest Ubuntu as the base image
FROM ubuntu:latest

# Update APT package list and upgrade installed packages
RUN apt-get update && apt-get upgrade -y

# Install Python3 and pip3
RUN apt-get install -y python3 python3-pip

# Remove EXTERNALLY-MANAGED file to avoid pip installation error
RUN rm /usr/lib/python*/EXTERNALLY-MANAGED

# Install Flask using pip3
RUN pip3 install flask flask-cors

# Copy the Python app script to the container
COPY api.py /app/api.py

# Set the working directory
WORKDIR /app

# Define the command to run the Flask app
CMD ["python3", "api.py"]