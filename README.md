# db_oracledb_docker
Oracle Database 21c in Docker

Flow
Review Docker installation
Docker Hub — Authentication
Pull the Docker Image
Create & run the container
Connect to the database

Review Docker Installation

docker -v

Docker Hub — Authentication

docker login

Pull the Docker Image

docker pull container-registry.oracle.com/database/express:latest

Create & run the container

docker container create -it --name oracle-test -p 1521:1521 -e ORACLE_PWD=welcome123 container-registry.oracle.com/database/express:latest

docker start [container-name] or docker stop [container-name]

Database Info

host: localhost
port: 1521
username: system
password: welcome123
sid: xe
