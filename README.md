# Where the ISS at
A simple real-time graphical visualization of positional data of the International Space Station

## Description

This project aims to demonstrate the use of REST APIs and Event Streams to provide real-time online services.
The proposed web project is a simple live tracking system of the International Space Station (ISS).

The data is taken from a [free API](https://wheretheiss.at/).
We retrieve the data, store it in a H2 database, with the help of JPA, and present the information in a simple web-UI containing a world map.
All requests made by our clients are logged through Kafka.
The deployment is done using docker containers and all code is presented with the proper documentation.

## Instructions on how to run the code

1. Have installed Docker and Docker Compose.
2. On repository's root folder, build the docker containers and start them:
```shell
docker-compose build
docker-compose up -d
```
3. Open a browser, enter the address 'http://localhost:8080/' and enjoy the application.
7. [Optional] Check out the address 'http://localhost:5000/' to see the Kafka logs and events live in a simple web UI.

## Authors

The authors of this project are Filipe Pires and João Alegria, and the project was developed for the Software Engineering Course of the Master's degree in Informatics Engineering of the University of Aveiro.

For further information contact us at filipesnetopires@ua.pt or joao.p@ua.pt.
