# Docker 101 Workshop - Day 1

One Day workshop on understanding Docker

## Prerequisites
 - Machine/VM with linux
 - Docker  ( https://docs.docker.com/engine/install/ubuntu/ )
 - Docker Compose ( https://docs.docker.com/compose/install/compose-plugin/#installing-compose-on-linux-systems )
 - Git     ( https://www.makeuseof.com/install-configure-git-on-linux/ )
 - VS code IDE ( https://linuxize.com/post/how-to-install-visual-studio-code-on-ubuntu-20-04/ )
 - Internet Connection

## Workshop environment setup 
 - git pull 'repo-name'
 - cd 'repo-name'
    ```
        docker run -d -p 8081:80 dockersamples/101-tutorial
    ```
 - If docker is not installed in your Linux
    ```
        This script is meant for quick & easy install via:
        $ sh install-docker-and-docker-compose.sh
    ```
 - open up http://localhost:8081/ in your browser

## Docker
- By the end of this workshop you will understand following things
    - You will be Introduced to the concept of containerisation and why its required.
    - You will learn how to Build and run your own Containers.
    - You will learn how to Run Multiple Services with Docker Compose
    - You will learn how to Build and run PHP and NGNIX containers.

## Schedule

| Time          | Topics
|---------------|-------
| 09:00 - 09:30 |  [`Introduction/What we do ?`]
| 09:30 - 09:45 |  [`Video Session: Introduction to Docker and Containers`](docker_intro.md)
| 09:45 - 10:30 |  [`Simple Docker Commands`](simple_docker_commands.md)
| 10:00 - 10:30 |  [`Getting Started, Our Application`](getting_started.md)
| 10:00 - 11:00 |  [`Updating our App`](updating_our_app.md)
| 11:00 - 11:45 |  [`Sharing our App`](sharing_our_app.md)
| 11:45 - 01:00 |  [`Persisting our DB and Bind Mounts`](persisting_our_app.md)
| 01:00 - 02:00 |  [`Break`]
| 02:00 - 03:30 |  [`Multi-Container Apps`](multi_container_app.md)
| 03:00 - 05:00 |  [`Using Docker Compose`](using_docker_compose.md)
| 05:00 - 05:15 |  [`Q & A`]
| 05:15 - 05:30 |  [`Wrapping Up`]