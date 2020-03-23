# Software Engineering - Lab Project

## Contextualization

This repository contains the work done by the authors on the lab project for the course in Software Engineering of the MSc. in Informatics Engineering of the University of Aveiro.
The assignment is focused on all the main concepts and technological solutions addressed in the first part of the course: REST (consuming and deploying), JPA (persisting), Kafka Messaging (logging and event alarms).
The deployment is done using docker containers and all code is presented with the proper documentation.

## Authors

Filipe Pires, nmec. 85122

João Alegria, nmec. 85048

## Description

The project is about a live tracking system of the International Space Station (ISS).
The data is taken from the REST API at https://wheretheiss.at/.
We retrieve the data, store it in a H2 database, with the help of JPA, and present the information in a simple web-UI containing a world map.
All requests made by our clients are logged through Kafka.

## Instructions on how to run the code

1. Have installed Docker and Docker Compose.
2. On repository's root folder, build the docker containers and start them:
```shell
docker-compose build
docker-compose up -d
```
3. Open a browser, enter the address 'http://localhost:8080/' and enjoy the application.
7. [Optional] Check out the address 'http://localhost:5000/' to see the Kafka logs and events live in a simple web UI.

