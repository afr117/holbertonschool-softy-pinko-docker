
FROM ubuntu:latest

# Update APT and install Python3, Python3-pip, and Flask
RUN apt-get update -y && apt-get upgrade -y && \
    apt-get install -y python3 python3-pip && \
    pip3 install flask

# Set the working directory to /app
WORKDIR /app

# Copy the Python file to the Docker image
COPY ./api.py /app/api.py

# Expose port 5252
EXPOSE 5252

# Start the Flask app
CMD ["python3", "api.py"]

