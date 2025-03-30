Docker Usage

This project is containerized using Docker, which simplifies the process of building, running, and deploying the application across different environments. Below is an overview of how Docker is used in this project:

What Docker Image Is Used
The project uses a custom Docker image defined by the Dockerfile in the project root.
The base image is openjdk:11-jdk 
Building the Docker Image
To build the Docker image, run the following command in the project root:

docker build -t hello-java:latest .
This command tells Docker to build an image with the tag hello-java:latest using the instructions in the Dockerfile.

Running the Docker Container
After building the image, you can run the container using:

docker run -p 8080:8080 hello-java:latest
The -p 8080:8080 option maps port 8080 of the container to port 8080 on your host machine. Adjust the ports as needed based on your project configuration.
Once the container is running, you can access the application via http://localhost:8080 
