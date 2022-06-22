## Docker post-installation setup
Do the optional precodure configuration to work better with Docker.

### Run Docker as non-root user
To create the docker group and add your user:
1. Create the docker group.
```
sudo groupadd docker
```
2. Add your user to the docker group.
```
sudo usermod -aG docker $USER
```

3. Activate the changes to groups:
```
newgrp docker 
```
4. Verify that you can run docker commands without sudo.
```
docker images
```

<br />

## Docker Commands
Docker is a containerization system which packages and runs the application with its dependencies inside a container. There are several docker commands you must know when working with Docker.
### 1. Docker version
To find the installed docker version
Command:
```
docker  --version
``` 
Example:
```
docker --version
Docker version 20.10.12, build e91ed57
```

<br>

### 2. Downloading image
To work with any ocker image we need to download the docker image first.<br /> 
Command:
```
docker pull <IMAGE>
```
Example of pulling alpine:latest image
```
docker pull alpine:latest
```

<br>

### 3. List all the docker images
To list all the images that is locallt available in the host machine, simply run the below command. This will list all the docker images in the local system.
<br />
Command:
```
docker images
Example:
```
REPOSITORY  TAG  IMAGE ID       CREATED      SIZE
alpine     latest  c059bfaa849c 6 weeks ago  5.59MB
```
docker images
```

### 3. Run docker image
The docker run command first creates a writeable container layer over the specified image, and then starts it using the specified command.
<br>
Command:
```
docker run [options] <IMAGE>
```
> Explore options [here](https://docs.docker.com/engine/reference/run/)


Example of running alpine:latest image, the options -t allows us to acces the terminal and -i gets stdin stream added. Basicaly using -ti adds the terminal driver.
```
docker run -t -i alpine:latest
or
docker run -ti alpine:latest
```
