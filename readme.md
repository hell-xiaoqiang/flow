# Backend CICD 

## Description

This project includes a `backend.yaml` file for Kubernetes configuration and a `Dockerfile` for building a Docker image.

## Kubernetes Configuration

The `backend.yaml` file is a Kubernetes configuration file that sets up a Namespace, a Service, and a Deployment.

To apply this configuration to your Kubernetes cluster, use the `kubectl apply` command:

```bash
kubectl apply -f backend.yaml
```

This command will create the Namespace, Service, and Deployment as defined in the `backend.yaml` file.

## Docker Image Building

The `Dockerfile` includes instructions for building a Docker image from a Java base image, copying a JAR file into the image, and setting the entrypoint for the container.

To build the Docker image, navigate to the directory containing the `Dockerfile` and run the `docker build` command:

```bash
docker build -t your-image-name .
```

Replace `your-image-name` with the name you want to give to your Docker image.

To run a container from this image, use the `docker run` command:

```bash
docker run -p 8080:8080 your-image-name
```

This command will start a container and map port 8080 in the container to port 8080 on your host machine.

## Help

If you encounter any problems or have any questions, please open an issue in this repository.