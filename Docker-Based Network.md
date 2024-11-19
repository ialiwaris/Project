# Docker-Based Network Setup Project

This project demonstrates setting up a Docker environment with interconnected containers and networks based on the given architecture.

## Project Description

### Setup Overview:
- Installed Docker.
- Created three branches: `B1`, `B2`, `B3`.
- Ran six Nginx containers, each representing a user or server:
  - `user1`, `user2`, `user3`, `user4`, `user5`, and `user6`.
  - `user4` serves as a web server with Nginx installed.

### Connectivity:
- **Green lines** in the diagram indicate direct connections between branches.
- **Red lines** signify connections limited to their respective branches.

## Implementation Steps

### Step 1: Install Docker
```bash
sudo apt update
sudo apt install docker.io
```
### Step 2: Create Docker Networks
```bash
docker network create B1
docker network create B2
docker network create B3
```
### Step 3: Run Nginx Containers
Run containers and attach them to the networks:

# For Branch B1
```bash
docker run --name user1 --network B1 -d nginx
docker run --name user2 --network B1 -d nginx
```
# For Branch B2
```bash
docker run --name user3 --network B2 -d nginx
docker run --name user4 --network B2 -d nginx # Web server
```
# For Branch B3
```bash
docker run --name user5 --network B3 -d nginx
docker run --name user6 --network B3 -d nginx
```
### Step 4: Configure Connectivity
To allow cross-branch communication for selected containers, use the following commands:

```bash
docker network connect B1 user3
docker network connect B2 user5
docker network connect B3 user1
```
### Step 5: Verify Connections
To check the network connections for each container and ensure the configurations are correct, run the following commands:

```bash
docker network inspect B1
docker network inspect B2
docker network inspect B3
```
These commands will display the details of each network, including connected containers and their IP addresses.
## Bring Down the Containers
To stop and remove the containers:
### Stop all running containers
```bash
docker stop user1 user2 user3 user4 user5 user6
```
### Remove the containers
```bash
docker rm user1 user2 user3 user4 user5 user6
```
## The Network has been Created, and My Project is Complete!
# Thank You...
