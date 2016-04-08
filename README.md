# docker-compose stack for usenet services

## Instructions
- ```brew install docker-compose```
- ```docker-compose up -d```

## Data Warehouse
The concept of the 'data warehouse' in the docker-compose.yml file is a central docker host volume which stores the configuration files for each usenet service. e.g. ```/data/warehouse/[servicename]/config.ini```. 
