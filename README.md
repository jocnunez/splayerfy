# Spotify Player

## DOCKER

### Images
```bash
# Build Image (from the same path where we have Dockerfile)
docker build -t web-image .

# Check Images
docker images

# Remove Images
docker rmi web-image
```


### Containers
```bash
# Run Container from Image
docker run --name web-container -d -p 8080:80 web-image

# Check Containers (-a for stopped containers)
docker ps -a

# Remove Container
docker rm web-container
```