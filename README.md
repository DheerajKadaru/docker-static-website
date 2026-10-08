# Docker Static Website

A simple static website containerized using Docker and served using Nginx.

## Technologies Used

- HTML
- CSS
- Docker
- Nginx

## Project Structure

```text
docker-static-website/
├── index.html
├── style.css
├── Dockerfile
└── README.md

Dockerfile
The Dockerfile uses the lightweight Nginx Alpine image and copies the website files into the Nginx web root.
How to Run
1. Build the Docker Image
docker build -t static-website .

2. Run the Container
docker run -d -P --name static-website-container static-website

3. Check the Running Container
docker ps

Docker automatically maps the container's port 80 to an available host port.
4. Open the Website
Open the port shown by docker ps in your browser.
Example:
http://localhost:32768