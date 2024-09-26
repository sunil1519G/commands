# Docker Commands

Useful Docker commands for managing containers, images, and networks.

## Table of Contents
- [Container Management](#container-management)
- [Images](#images)
- [Network and Volumes](#network-and-volumes)

### Container Management
1. **List all containers**:
    ```bash
    docker ps -a
    ```

2. **Start/Stop a container**:
    ```bash
    docker start <container>
    docker stop <container>
    ```

3. **Access container shell**:
    ```bash
    docker exec -it <container-name> bash
    ```

### Images
1. **Remove specific images**:
    ```bash
    docker rmi <image-1> <image-2> ...
    ```

2. **Remove all images**:
    ```bash
    docker rmi $(docker images -q)
    ```


### Logs
1. **View container logs**:
   ```bash
   docker container logs <container-name>
   ```
   
2. **Follow live logs from a container**:
   ```bash
   docker logs -f <container-name>
   ```


### Network and Volumes
1. **Run MySQL container with network**:
    ```bash
    docker run --name mysql-container --network my_network -e MYSQL_ROOT_PASSWORD=root -d mysql:latest
    ```

