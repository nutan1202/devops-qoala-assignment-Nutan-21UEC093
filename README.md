# devops-qoala-assignment-Nutan-21UEC093
# Project Setup

This project utilizes Docker to effectively containerize the application. Below are the essential modifications made to various Docker and configuration files to enhance functionality and accuracy.
## Changes Made

### 1. `docker-compose.yaml`

* **Port Number Correction**: Changed the port mapping from `"eighty:80"` to `"80:80"` to use numeric values.
* **Path Correction**: Updated the path from `.confi` to `.conf`.
* **Port Update**: Revised the port specification from `"eight thousand"` to `8000`.
* **Network Driver Correction**: Corrected the spelling of the network driver from `"bridg"` to `"bridge"`.
* **Command Change**: Replaced `expose` with `ports` to allow public access to the specified port.

### 2. `nginx/Dockerfile`

* **Version Tag Update**: Changed `FROM nginx:latests` to `FROM nginx:latest`.
* **Image Name Typo Fix**: Corrected `"nginix"` to `"nginx"`.
* **HTML Directory Removal**: Removed the line `COPY ./html /usr/share/nginx/html` since there are no HTML files to copy.
* **Port Number Correction**: Updated the port from `"Eighty"` to `80`.
* **Command Fix**: Corrected the command from `"daemon of;"` to `"daemon off;"`.

### 3. `nginx/nginx.conf`

* **Worker Processes**: Fixed `worker_process auto` to `worker_processes auto`.
* **MIME Types Typo**: Corrected `"mime.typess"` to `"mime.types"`.
* **Default Type Typo**: Changed `"default_typ"` to `"default_type"`.

### 4. `Python/Dockerfile`

* **Directory Name Correction**: Changed `"appp"` to `"app"`.
* **App File Name**: Corrected `"appy.py"` to `"app.py"`.
* **Library Name Fix**: Changed the library name from `"netiface"` to `"netifaces"`.
* **Port Number Update**: Revised the port from `"eight thousand"` to `8000`.
* **Command Correction**: Updated the command from `"pythn"` to `"python"`.
## Troubleshooting Docker Errors

During the setup and running of the Docker container, I encountered the following errors:
### 1.Spelling errors:
* **Error**: failed to solve: nginx:latests: failed to resolve source metadata for docker.io/library/nginx:latests: not found
* **Resolution**: This error indicated a typo in the image name. The correct tag for the Nginx image is latest, not latests.

### 2.No html file:
* **Error**: failed to solve: failed to compute cache key: failed to calculate checksum of ref 35eb6f41-e46c-48e9-ac53-a00aab0dfad2::q5gecu70mqlwf8174plg0xr9e: "/html": not found
* **Resolution**: This error occured because the specified directory or file to copy does not exist. I made sure that the html directory exists in the same directory as your Dockerfile. As it was not present I commented the line.

## Screenshots

Here are relevant screenshots:

### Docker Running Container
![Docker Running Containers](Screenshots/Running%20containers.png)

### App Running in Browser
![App Running in Browser](Screenshots/Browser%20showing%20running%20Application.png)

### Logs of the requests
![Logs of the requests](Screenshots/Logs%20of%20the%20requests.png)

### Terminal showing created containers
![Terminal showing created containers](Screenshots/Terminal%20showing%20created%20containers.png)

### HTML Error Screenshot
![HTML Error Screenshot](Screenshots/Error%20encountered%20due%20to%20known%20html%20file.png)

### Project File on Docker
![Project File on Docker](Screenshots/Project%20opened%20in%20docker.png)
