# app
TheEyeDashboard application (Docker-compose)

## Build and run TheEyeDashboard app

```bash
docker-compose build
docker-compose up
```

## Build in development

```bash
docker-compose -f development.yml build
docker-compose -f development.yml up
```
In development, microservices are built from source + Dockerfiles instead of images.
Make sure all to have all symbolic links to microservices in /dev_links

Ex : ./links/datasource_manger should point to existing datasource_manger repository.

List of all microservices to link : https://github.com/theeyedashboard
