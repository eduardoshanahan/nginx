# Nginx

A Docker image with [Nginx](https://nginx.org/en/)

## Building

```bash
docker build -t eduardoshanahan/nginx .
```

## Running a test

```bash
docker run --rm -p 8080:80 -v content:/usr/share/nginx/html:ro -d eduardoshanahan/nginx:latest
```

## Development

If you want to make some changes and version it, [bumpversion](https://pypi.python.org/pypi/bumpversion) is available

```bash
bumpversion patch
```
