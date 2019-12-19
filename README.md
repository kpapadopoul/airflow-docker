# Airflow Docker

## Build the Docker image
```bash
docker build . -t airflow
```

## Create and Run the container (do this only when image is rebuilt)
```bash
docker run -d -p 8080:8080 -v c:/Users/uoclo/IdeaProjects/airflow/docker/dags:/app/airflow/dags --rm --name airflow_container airflow
```

## Connect to the container
```bash
docker exec -it airflow_container /bin/bash
```

## Stop the container
```bash
docker stop airflow_container
```

## Restart the container
```bash
docker start airflow_container