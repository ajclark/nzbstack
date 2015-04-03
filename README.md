# docker-compose stack for usenet services

## Instructions
- Install docker-compose
- ```docker-compose up -d```

## Data Warehouse
The concept of the 'data warehouse' in the docker-compose.yml file is a central docker host volume which stores the configuration files for each usenet service. e.g. ```/data/warehouse/[servicename]/config.ini```. It was coined by @lngarrett

## Disclaimer
Bundling the Dockerfiles for different services under a single repository sucks, as it complicates publishing images to the Docker Hub, but this seems to be the 'cleanest' way of organizing multiple services for docker-compose.
