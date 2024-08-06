# Linux Sysadmin Learning Environment with Docker

## Overview

This project sets up two Ubuntu 22.04 containers using Docker and Docker Compose for learning Linux system administration.

### Containers

- **Server Container:**
  - Essential tools: `vim`, `nano`, `ifconfig`
  - Services: `nginx`, `openssh-server`, `vsftpd`

- **Client Container:**
  - Essential tools: `vim`, `nano`, `ifconfig`
  - Client applications: `curl`, `openssh-client`, `lftp`

### Steps

1. **Create Dockerfiles:**
   - `Dockerfile.server` for the server container.
   - `Dockerfile.client` for the client container.

2. **Create `vsftpd.conf`** for FTP server configuration.

3. **Create `docker-compose.yml`** to define and run multi-container Docker applications.

4. **Build and Run Containers:**
   - Use `docker-compose up -d` to build and run the containers.

5. **Access the Server from the Client:**
   - Exec into the client container and test access to server services (SSH, web server, FTP).