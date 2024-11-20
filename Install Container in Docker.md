# Installing Containers in Docker

Docker is a platform for developing, shipping, and running applications inside **containers**. A **container** is a lightweight, standalone, and executable package that includes everything needed to run a piece of software, including the code, runtime, libraries, and system tools.

To run applications using Docker, you need to create or pull a **container** image, and then you can **run** it as a **container**.
# Let's Install...
## Steps to Install and Run a Docker Container
### 1. **Pull the Nginx Docker Image**
First, pull the official Nginx image from Docker Hub:
```bash 
docker pull nginx
```
### 2. **Run the Nginx Container**
Once the image is downloaded, you can run the Nginx container. The following command runs the Nginx container in detached mode and maps port 80 on your host to port 80 on the container:
```bash
docker run -d -p 80:80 nginx
```
- `-d` runs the container in **detached mode** (in the background).
- `-p 80:80` maps port 80 of your host to port 80 of the container, allowing you to access Nginx via `localhost:80`.
### 3. **Verify the Nginx Container is Running**
To check if the Nginx container is running, use the following command:
```bash
docker ps
```
This command will list all running containers, and you should see Nginx listed there.

### 4. **Access the Nginx Server**
Open your browser and navigate to your server's IP address or localhost (if running locally):
```bash
http://localhost
```
You should see the default Nginx welcome page, confirming that the container is running properly.

## If You Need to Stop Nginx Container:
```bash
docker stop <container_id_or_name>
```
## If You Need to Remove Nginx Container:
```bash
docker rm <container_id_or_name>
```
# These steps will allow you to install, run, and manage an Nginx container in Docker!
# Thank You...
