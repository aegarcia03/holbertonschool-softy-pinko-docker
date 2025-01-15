# Use the latest Ubuntu image as the base
FROM ubuntu:latest

RUN apt-get update \
    apt-get upgrade -y && \
    apt-get install -y python3 && \
    apt-get install -y python3-dev && \
    apt-get install -y python3-pip

# Install Flask
RUN pip3 install flask
RUN pip3 install flask-cors

# Set the working directory to /app
WORKDIR /app

# Copy api.py into the /app directory inside the Docker container
COPY ./api.py /app/api.py

# Expose the port 5252
EXPOSE 5252

# Run Flask app on host
CMD ["python3", "api.py"]

#Build the Docker Image : docker build -t softy-pinko:task1 .