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
