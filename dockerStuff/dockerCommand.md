<h1>Docker Commands</h1>
<h2>Build an image</h2>

`docker build -t <image name:version> -f <dockerfile path> .`
<h2>Run an image</h2>

`docker run [OPTIONS] IMAGE [COMMAND] [ARG...]`
- frequently used options:
	- -it (interactive)
	- -d (detached in the background)
	- --name (container name)


<h2>Running Commands in the container using exec</h2>

`docker exec -it <container-name> /bin/sh`


<h2>Running Commands in the container using run</h2>

`docker run -it <image-name> /bin/sh`

<h2>Pull an image</h2>

`docker pull <image-name>:version`

<h2>Push an image</h2>

`docker push <image:name>:version`

<h2>Login</h2>

`docker login`

<h2>Logs</h2>

`docker logs [OPTIONS] CONTAINER`

<h2>Delete an image</h2>

`docker image rm <image-name>:version`
- use -f for force remove

<h2>Delete a container</h2>

`docker rm [OPTIONS] CONTAINER [CONTAINER...]`
- use -f for force remove

<h2>Start a container</h2>

`docker start [OPTIONS] CONTAINER [CONTAINER...]`

<h2>Stop a container</h2>

`docker stop [OPTIONS] CONTAINER [CONTAINER...]`

<h2>See the running container list</h2>

`docker ps`
- use --all for all types of container

<h2>Inspect an image</h2>

`docker image inspect <image:name>:version`

<h2>Mount a path in the container</h2>

`docker run -t -i -v <host_dir>:<container_dir>  ubuntu /bin/bash`
