Apologies for the confusion earlier! Here's the `README.md` file with all Docker commands in the proper markdown section format:

```markdown
# Docker Commands Cheat Sheet

This document contains a list of commonly used Docker commands for development and deployment.

## Docker Commands

### Docker Installation
- Install Docker on your system:
  - **Windows**: [Docker Desktop](https://www.docker.com/products/docker-desktop)
  - **Linux**: Follow the [installation guide](https://docs.docker.com/engine/install/)
  - **macOS**: [Docker Desktop for Mac](https://www.docker.com/products/docker-desktop)

### Basic Docker Commands

- **Check Docker version:**
  ```bash
  docker --version
  ```

- **Display system-wide Docker information:**
  ```bash
  docker info
  ```

### Docker Container Commands

- **List running containers:**
  ```bash
  docker ps
  ```

- **List all containers (running and stopped):**
  ```bash
  docker ps -a
  ```

- **Start a stopped container:**
  ```bash
  docker start <container_id>
  ```

- **Stop a running container:**
  ```bash
  docker stop <container_id>
  ```

- **Restart a running container:**
  ```bash
  docker restart <container_id>
  ```

- **Remove a stopped container:**
  ```bash
  docker rm <container_id>
  ```

- **Remove all stopped containers:**
  ```bash
  docker container prune
  ```

- **Execute a command inside a running container:**
  ```bash
  docker exec -it <container_id> bash
  ```

### Docker Image Commands

- **List all Docker images:**
  ```bash
  docker images
  ```

- **Pull an image from Docker Hub:**
  ```bash
  docker pull <image_name>
  ```

- **Build a Docker image:**
  ```bash
  docker build -t <image_name>:<tag> .
  ```

- **Remove a Docker image:**
  ```bash
  docker rmi <image_id>
  ```

### Docker Network Commands

- **List Docker networks:**
  ```bash
  docker network ls
  ```

- **Create a Docker network:**
  ```bash
  docker network create <network_name>
  ```

- **Remove a Docker network:**
  ```bash
  docker network rm <network_name>
  ```

### Docker Volume Commands

- **List Docker volumes:**
  ```bash
  docker volume ls
  ```

- **Create a Docker volume:**
  ```bash
  docker volume create <volume_name>
  ```

- **Remove a Docker volume:**
  ```bash
  docker volume rm <volume_name>
  ```

### Docker Compose Commands

- **Start services defined in the `docker-compose.yml` file:**
  ```bash
  docker-compose up
  ```

- **Start services in detached mode (in the background):**
  ```bash
  docker-compose up -d
  ```

- **Stop and remove services defined in the `docker-compose.yml` file:**
  ```bash
  docker-compose down
  ```

- **View logs for all services in the `docker-compose.yml` file:**
  ```bash
  docker-compose logs
  ```

### Docker System Commands

- **Clean up unused data (stopped containers, unused networks, dangling images):**
  ```bash
  docker system prune
  ```

- **Clean up unused Docker images:**
  ```bash
  docker image prune
  ```

- **Clean up unused Docker volumes:**
  ```bash
  docker volume prune
  ```

### Docker Buildx (Multi-architecture Builds)

- **Build an image for multiple architectures:**
  ```bash
  docker buildx build --platform linux/amd64,linux/arm64 -t <image_name> .
  ```

### Docker Logs Commands

- **View logs for a specific container:**
  ```bash
  docker logs <container_id>
  ```

- **Tail logs for a container:**
  ```bash
  docker logs -f <container_id>
  ```

### Docker Tag Commands

- **Tag an image with a new name and tag:**
  ```bash
  docker tag <image_id> <new_image_name>:<tag>
  ```

### Docker Push Commands

- **Push an image to Docker Hub:**
  ```bash
  docker push <image_name>:<tag>
  ```

### Docker Build Arguments

- **Pass build arguments to the Docker build process:**
  ```bash
  docker build --build-arg <key>=<value> -t <image_name> .
  ```




### Join my Organization: 
Link: <a href="https://github.com/Tech-Hubs" target="_blank">PrabhatDevLab</a>


<p>Happy Learning! 📚✨ Keep exploring and growing your knowledge! 🚀😊</p>
