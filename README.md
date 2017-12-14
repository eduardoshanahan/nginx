# Nginx

A Docker image with [Nginx](https://nginx.org/en/), based in [Docker Nginx](https://hub.docker.com/r/_/nginx/)

## Building

```
docker build . -t eduardoshanahan/nginx:latest
```

## Running an interactive test

```
docker run --rm -p 8080:80 -v $(pwd)/content:/usr/share/nginx/html:ro eduardoshanahan/nginx:latest
```

Or with Docker Compose

```
docker-compose up
```

Then you can curl to:

```
curl localhost:8080
```

## Building an image in Docker Hub

If for any reason the tagged build fails, you can fire a fresh one running

```
./build_image.sh
```

## Development

To send the commits to the remote server, you can use the script

```
./save.sh
```

which will also create a new tag if the version is updated.
