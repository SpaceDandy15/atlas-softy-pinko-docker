# Use the latest Ubuntu image as the base
FROM ubuntu:latest

# Set environment variables to avoid interactive prompts during installation
ENV DEBIAN_FRONTEND=noninteractive

# Update the package list and install necessary packages
RUN apt-get update && \
    apt-get install -y --no-install-recommends python3 python3-pip && \
    rm -rf /var/lib/apt/lists/*

# Install Flask using pip3
RUN pip3 install --no-cache-dir flask

# Set /app as the working directory
WORKDIR /app

# Copy the Python file to the working directory
COPY ./api.py .

# Expose the port your Flask app runs on (default is 5000)
EXPOSE 5000

# Run the Flask app
CMD ["python3", "api.py"]

