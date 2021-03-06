# Docker Webserver
Custom docker image used for learning custom image building, and used in my [Kubernetes Cluster Build](https://github.com/TheQuib/k3s)

# What does this use?
 - Docker
   - Uses base image `nginx:alpine`

# Prebuilt Image
You can find a prebuilt image right here on GitHub at  [ghcr.io/thequib/nginx-docker:latest](http://ghcr.io/thequib/nginx-docker:latest)
 - Or run `docker pull ghcr.io/thequib/nginx-docker:latest` to get it now

# Build it Yourself
 - Clone the repository
 - Run the command `sudo docker build -t webserver:latest .`
   - This will create a container on the local machine called `webserver` with the tag `latest`
   - Just as if downloaded from a Docker repository such as Dockerhub
 - Now that the container is built, run the command `sudo docker run -d webserver:latest`
   - This will run the container is 'detached' mode, in the background
 - Alternatively, the included `docker-compose.yml` file can be used if you prefer by running `sudo docker-compose up -d`