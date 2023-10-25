# Python image for docker with debian 11
## Build your image
```
DOCKER_BUILDKIT=1 docker build -t python-custom .
```
## Using the image you built, now you run your service
```
DOCKER_BUILDKIT=1 docker build -t ws-taller .
```

## Run your service
```
 docker run --name ws-taller --restart unless-stopped --env-file C:/Users/GFDP/Documents/Services/ws-taller/.env --network=services_default --link msyql -p 8000:8000 ws-taller:latest
```

