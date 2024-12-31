
# Docker Commands Cheat Sheet

This document contains a list of commonly used Docker commands for development and deployment.

## Docker Commands

### Docker Installation
- Install Docker on your system:
  - **Windows**: [Docker Desktop](https://www.docker.com/products/docker-desktop)
  - **Linux**: [installation guide](https://docs.docker.com/engine/install/)
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

---

## Additional Commands

### Java JShell Commands

- **Start Java JShell:**
  ```bash
  jshell
  ```

- **Run a Java program from a file:**
  ```bash
  jshell <path_to_file>.java
  ```

- **Exit Java JShell:**
  ```bash
  /exit
  ```

- **Display current variables and methods in JShell:**
  ```bash
  /vars
  /methods
  ```

### Running Java Code in Docker

- **Create a Dockerfile for Java:**
  ```dockerfile
  FROM openjdk:17-jdk-alpine
  COPY . /app
  WORKDIR /app
  RUN javac HelloWorld.java
  CMD ["java", "HelloWorld"]
  ```

- **Build a Docker image for a Java program:**
  ```bash
  docker build -t java-app .
  ```

- **Run a Java program in Docker:**
  ```bash
  docker run java-app
  ```

### MySQL Commands

- **Run MySQL Docker container:**
  ```bash
  docker run --name mysql-container -e MYSQL_ROOT_PASSWORD=rootpassword -d mysql:latest
  ```

- **Access MySQL container:**
  ```bash
  docker exec -it mysql-container mysql -uroot -p
  ```

- **Run MySQL query inside container:**
  ```bash
  docker exec -it mysql-container mysql -uroot -prootpassword -e "SELECT * FROM mydatabase.mytable;"
  ```

- **Stop MySQL container:**
  ```bash
  docker stop mysql-container
  ```

- **Remove MySQL container:**
  ```bash
  docker rm mysql-container
  ```



### Key Additions:
1. **Java JShell** commands for running Java code interactively.
2. **Running Java code in Docker** — how to containerize and run a simple Java application.
3. **MySQL commands** to interact with MySQL containers for database queries.




---


## Click here to get in touch with me: 
<a href="https://github.com/Tech-Hubs" target="_blank"><b>PrabhatDevLab</b></a>, 
<a href="https://hugs-4-bugs.github.io/myResume/" target="_blank"><b>PrabhatKumar.com</b></a>, 
<a href="https://www.linkedin.com/in/prabhat-kumar-6963661a4/" target="_blank"><b>LinkedIn</b></a>, 
<a href="https://stackoverflow.com/users/19520484/prabhat-kumar" target="_blank"><b>Stackoverflow</b></a>, 
<a href="https://github.com/Hugs-4-Bugs" target="_blank"><b>GitHub</b></a>, 
<a href="https://leetcode.com/u/Hugs-2-Bugs/" target="_blank"><b>LeetCode</b></a>, 
<a href="https://www.hackerrank.com/profile/Prabhat_7250" target="_blank"><b>HackerRank</b></a>, 
<a href="https://www.geeksforgeeks.org/user/stealthy_prabhat/" target="_blank"><b>GeeksforGeeks</b></a>, 
<a href="https://hugs-4-bugs.github.io/AlgoByPrabhat/" target="_blank"><b>AlgoByPrabhat</b></a>, 
<a href="http://hugs-4-bugs.github.io/Sharma-AI/" target="_blank"><b>SHARMA AI</b></a>,  <a href="https://linktr.ee/_s_4_sharma" target="_blank"><b>About Me</b></a>, <a href="https://www.instagram.com/_s_4_sharma/" target="_blank"><b>Instagram</b></a>, <a href="https://x.com/kattyPrabhat" target="_blank"><b>Twitter</b></a>


<p>Happy Learning! 📚✨ Keep exploring and growing your knowledge! 🚀😊</p>
