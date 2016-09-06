# Nginx

A Docker image with [Nginx](https://nginx.org/en/), based in [Docker Nginx](https://hub.docker.com/r/_/nginx/)

## Building

```bash
docker build -t eduardoshanahan/nginx .
```

## Running a test

```bash
docker run --rm -p 8080:80 -v $(pwd)/content:/usr/share/nginx/html:ro eduardoshanahan/nginx:latest
```

Or you can use Docker Compose:

```bash
docker-compose up
```

Then you can curl to:

```bash
curl localhost:8080
```

## Development

If you want to make some changes and version it, [bumpversion](https://pypi.python.org/pypi/bumpversion) is available

```bash
bumpversion patch
```
