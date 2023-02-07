# React basic template | docker | docker-compose

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app) and cleaned from unnecessary files.

## Available Scripts

In the project directory, you can run:

### ```docker-compose up -d```
It will be a docker image based on ```Dockerfile.dev``` file.\
Each update will be automatically replicated inside the docker container, so you don't need to rebuild the image every time.\
Add ```-d``` if you want to run the container in detached mode.

### ```docker-compose down```
It will stop the docker container.

### ```docker build -t <image-name>:<tag> .```
It will build a production docker image using a multi-phase building based on the result of ```npm run build``` and nginx docker image.

### ```docker run -d -p 80:80 <image-name>:<tag>```
It will start the docker container in production mode.\
Add ```-d``` if you want to run the container in detached mode.

### ```docker stop <container-id>```
It will stop the docker container.
