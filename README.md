# docker-test-app

A minimal Go HTTP server for testing container builds and deployments.

- `GET /` returns `Hello from <hostname>`
- `GET /healthz` returns `ok`
- Listens on `$PORT` (default `8080`)

```sh
docker build -t docker-test-app .
docker run --rm -p 8080:8080 docker-test-app
curl localhost:8080
```
