# Demo Wordpress Setup Using Docker
## with docker compose using three service: 
### official wordpress image
### official mysql image
### dbeaver as db viewer on port 5021 
### feel free to use any other image (e.g: phpmyadmin) 
### Make sure all running on the same network

### Before running the containers create network first:
```console
docker network create mylocalnetwork
```
#### Make sure you define your env values in .env file



#### Inside docker-compose.yml directory run:
```console
docker compose up
```
### Or if you need to run in the background withour blocking the terminal run:
```console
docker compose up -d
```

#### My docker and docker compose versions:

#### Docker Engine - Community
#### Version: 24.0.7

#### Docker Compose 
#### version v2.21.0

A note you can avoid exposing any ports on any containers on your server
and you can have reverse proxy service on the same network to proxy traffic to wordpress
without exposing any unneeded ports