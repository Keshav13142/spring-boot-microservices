# Spring boot and Microservice with Kubernetes

## Building image

```sh
mvn clean install && docker build -t image_name:latest
```

## Running containers

```sh
docker run -d -p port:port --name container_name -e CONFIG_SERVER_URL=http://host.docker.internal:9296  -e EUREKA_SERVER_ADDRESS=http://host.docker.internal:8761/eureka image_name
```
