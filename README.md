# Docker 101 Workshop - Day 1

One Day workshop on understanding Docker and Containers. Learn to run a container, inspect a container and understand the isolation of processes. Create a Dockerfile, and build an image from a Dockerfile. Learn how to mount application code using volume mount. Learn how to make your app data persistent across multiple containers. Learn how to create multiple containers from a single image, run multiple containers using docker-compose, and more.

## Prerequisites
 - Ubuntu 20.04 LTS  ( https://releases.ubuntu.com/focal/ubuntu-20.04.5-desktop-amd64.iso )
 - Docker  ( https://docs.docker.com/engine/install/ubuntu/#install-using-the-convenience-script )
 - Git     ( https://www.atlassian.com/git/tutorials/install-git#linux )
   - Create github account (https://github.com/signup)
   - Setting up SSH key with GitHub for Ubuntu
 (https://medium.com/featurepreneur/setting-up-ssh-key-with-github-for-ubuntu-cd8f2fabf25b)
 - VS code IDE ( https://linuxize.com/post/how-to-install-visual-studio-code-on-ubuntu-20-04/ )
 - Internet Connection and Chrome browser.

## Workshop environment setup 
 - Check if Git, Docker, and Docker Compose are installed in on the system. Open the terminal and run the following command
   ```
   mis@mispl-lap-31:~$ git --version
   git version 2.25.1

   mis@mispl-lap-31:~$ docker --version
   Docker version 20.10.17, build 100c701

   mis@mispl-lap-31:~$ docker compose version
   Docker Compose version v2.6.0

   ```
 - Open terminal and run following command to create a folder called workshop
    ```
    mkdir workshop
    ```
 - Navigate to the folder workshop and clone the from your personal repo using git
    ```
    cd workshop
    ```
 - Clone Website-Workshop1 repo && go inside Webiste-Workshop1 folder
    ``` 
    git clone git@github.com:<YOUR-GIT-ID>/Website-Workshop1.git
    cd Website-Workshop1
    ```
 - To open folder in VS code editor
    ```
    cd ~/workshop/Website-Workshop1
    code .
    ```
 - If docker is not installed in your Linux run the following command
    ```
    $ curl -fsSL https://get.docker.com -o get-docker.sh
    $ sudo sh get-docker.sh
   ```
 - Download dockersamples/101-tutorial image and bring up the container
    ```
    sudo docker run -d -p 8081:80 dockersamples/101-tutorial
    ```

 - open up http://localhost:8081/ in your browser

## What will you learn by the end of this workshop?
- By the end of this workshop, you will learn what docker is and understand how to set up containers.
- You will be introduced to containerization concepts and why it is required.
- You will learn how to build and run your own Containers.
- You will learn how to run Multiple Services with Docker Compose.
- You will learn how to build and run PHP and NGNIX containers.

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
