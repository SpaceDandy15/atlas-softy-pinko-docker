# Use the latest Ubuntu image as the base
FROM ubuntu:latest

# Update the package list and upgrade the installed software
RUN apt-get update && apt-get upgrade -y

# Install Python3 and pip3
RUN apt-get install -y python3 python3-pip

# If you encounter the "externally managed" error, remove the EXTERNALLY-MANAGED file
RUN rm /usr/lib/python*/EXTERNALLY-MANAGED || true

# Install Flask using pip3
RUN pip3 install flask

# Set /app as the working directory
WORKDIR /app

# Copy the Python file to the working directory
COPY ./api.py /app/api.py

# Run the Flask app
CMD ["python3", "api.py"]
