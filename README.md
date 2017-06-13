Docker Compose template
===

docker compose template collection, use [jwilder/nginx-proxy](https://github.com/jwilder/nginx-proxy)

|app|armhf image|amd64 image|
|-|-|-|
|nginx-proxy|yangxuan8282/rpi-nginx-proxy, [docker compose](https://github.com/yangxuan8282/docker-recipes/blob/master/armhf/nginx-proxy/docker-compose.yml)|jwilder/nginx-proxy, [docker compose](https://github.com/yangxuan8282/docker-recipes/blob/master/amd64/nginx-proxy/docker-compose.yml)|
|portainer|portainer/portainer, [docker compose](https://github.com/yangxuan8282/docker-recipes/tree/master/armhf/portainer)|portainer/portainer, [docker compose](https://github.com/yangxuan8282/docker-recipes/tree/master/amd64/portainer)|
|ghost|alexellis2/ghost-on-docker, [docker compose](https://github.com/yangxuan8282/docker-recipes/blob/master/armhf/ghost/docker-compose.yml)|ghost, [docker compose](https://github.com/yangxuan8282/docker-recipes/blob/master/amd64/ghost/docker-compose.yml)|
|tale|_|pipill/tale, [docker compose](https://github.com/yangxuan8282/docker-recipes/blob/master/amd64/tale/docker-compose.yml)|
|gogs|gogs/gogs-rpi, [docker compose](https://github.com/yangxuan8282/docker-recipes/blob/master/armhf/gogs/docker-compose.yml)|gogs/gogs, [docker compose](https://github.com/yangxuan8282/docker-recipes/blob/master/amd64/gogs/docker-compose.yml)|
|gitlab|yangxuan8282/rpi-gitlab, [docker compose](https://github.com/yangxuan8282/docker-recipes/blob/master/armhf/gitlab/docker-compose.yml)|gitlab, [docker compose](https://github.com/yangxuan8282/docker-recipes/blob/master/amd64/gitlab/docker-compose.yml)|
|drone|_|drone/drone, [docker compose](https://github.com/yangxuan8282/docker-recipes/blob/master/amd64/droneci/docker-compose.yml)|
|nexcloud|yangxuan8282/armhf-nextcloud, [docker compose](https://github.com/yangxuan8282/docker-recipes/tree/master/armhf/nextcloud)|nexcloud, [docker compose](https://github.com/yangxuan8282/docker-recipes/tree/master/amd64/nextcloud)|
|owncloud|yangxuan8282/armhf-owncloud, [docker compose](https://github.com/yangxuan8282/docker-recipes/tree/master/armhf/owncloud)|owncloud, [docker compose](https://github.com/yangxuan8282/docker-recipes/tree/master/amd64/owncloud)|
|seafile|sunx/seafile|sunx/seafile|
|h5ai|yangxuan8282/rpi-alpine-h5ai, [docker compose](https://github.com/yangxuan8282/docker-recipes/blob/master/armhf/h5ai/docker-compose.yml)|bixidock/h5ai, [docker compose](https://github.com/yangxuan8282/docker-recipes/blob/master/amd64/h5ai/docker-compose.yml)|
|minio|minio/minio, [docker compose](https://github.com/yangxuan8282/docker-recipes/tree/master/armhf/minio)|minio/minio, [docker compose](https://github.com/yangxuan8282/docker-recipes/tree/master/amd64/minio)|
|btsync|yangxuan8282/rpi-resilio-sync|resilio/sync|
|leanote|yangxuan8282/armhf-leanote|zuolan/leanote, [docker compose](https://github.com/yangxuan8282/docker-recipes/blob/master/amd64/leanote/docker-compose.yml)|
|tekki|_|teakki/teakki, [docker compose](https://github.com/yangxuan8282/docker-recipes/blob/master/amd64/teakki/docker-compose.yml)|
|aria2|yangxuan8282/rpi-alpine-aria2|_|
|fail2ban|_|superitman/fail2ban, [docker compose](https://github.com/yangxuan8282/docker-recipes/blob/master/amd64/fail2ban/docker-compose.yml)|
|linux dash|_|itxaka/linux-dash-docker, [docker compose](https://github.com/yangxuan8282/docker-recipes/blob/master/amd64/linux-dash/docker-compose.yml)|
|privatebin|yangxuan8282/privatebin, [docker compose](https://github.com/yangxuan8282/docker-recipes/blob/master/armhf/privatebin/docker-compose.yml)|jgeusebroek/privatebin, [docker compose](https://github.com/yangxuan8282/docker-recipes/blob/master/amd64/privatebin/docker-compose.yml)|
|shadowsocks|_|imhang/kcp-shadowsocks-docker, [docker compose](https://github.com/yangxuan8282/docker-recipes/blob/master/amd64/ss/docker-compose.yml)|


create network first:

```
docker network create proxy-network
```

then start `nginx-proxy` with docker compose template

next start `portainer` with docker compose template

finally start all your apps