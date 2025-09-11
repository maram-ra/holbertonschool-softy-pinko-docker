# Use Ubuntu as the base image
FROM ubuntu:latest

# Update packages and install Python and pip
RUN apt-get update && apt-get upgrade -y && apt-get install -y python3 python3-pip

# Optional: Remove externally-managed restrictions if present
RUN rm -f /usr/lib/python*/EXTERNALLY-MANAGED || true

# Install Flask using pip3
RUN pip3 install flask

# Set the working directory inside the container
WORKDIR /app

# Copy the Flask application code into the container
COPY ./api.py /app/api.py

# Run the Flask application
CMD ["python3", "api.py"]
