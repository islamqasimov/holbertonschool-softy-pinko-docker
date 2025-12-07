# Base image
FROM ubuntu:latest

# Update and upgrade packages
RUN apt-get update && apt-get upgrade -y

# Install Python3 and pip3
RUN apt-get install -y python3 python3-pip

# Fix EXTERNALLY-MANAGED issue if it occurs
RUN rm -f /usr/lib/python*/EXTERNALLY-MANAGED

# Install Flask using pip3
RUN pip3 install flask

# Set working directory
WORKDIR /app

# Copy API file into container
COPY ./api.py /app/api.py

# Run the Flask API when the container starts
CMD ["python3", "api.py"]
