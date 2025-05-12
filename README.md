# Hello Python (Dockerized)

A lightweight and containerized Python application, designed to be easily deployable using Docker. All dependencies are managed inside the container, making it a hassle-free setup on any system with Docker installed.

## Project Structure

```
app/                 # Your main Python application code
Dockerfile           # Docker configuration to build the image
requirements         # Python dependencies (used by pip install -r)
```

## How to Use

You only need two commands to get this running on your system using Docker:

```bash
docker pull parasminfy/hello-python:latest
docker run -p 8000:8000 parasminfy/hello-python:latest
```

## Building the Image Locally (Optional)

If you'd rather build the image yourself:

```bash
docker build -t hello-python .
docker run -p 8000:8000 hello-python
```

## Notes

- Ensure port `8000` matches what your app exposes.
- The `requirements` file should include all necessary Python libraries.
- Adjust the Dockerfile or ports if your app uses different settings.
