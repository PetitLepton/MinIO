To run a container, create the `minio` folder as user `$(id -u)` first and then
```
MINIO_ROOT_USER=... MINIO_ROOT_PASSWORD=... UID_=$(id -u) GID_=$(id -g) docker-compose run --rm minio
```