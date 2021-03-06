# The Eye Dashboard application

![ThEyeDashboard](docs/theeye.png)

## Build and run the app with Docker

This is the main app microservice.
It orchestrates all other microservices.

```bash
docker-compose build
docker-compose up
```

## Build in development

```bash
docker-compose build
docker-compose up
```

In development, microservices are built from source + Dockerfiles instead of images.
Make sure all to have all symbolic links to microservices in /dev_links

Ex : ./links/datasource_manger should point to existing datasource_manger repository.

List of all microservices to link : https://github.com/theeyedashboard

## Build in production
```bash
docker-compose -f production.yml build
docker-compose -f production.yml up
```
