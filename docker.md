# Docker cheat Sheet

### Installing Docker at Ubuntu 18.04:
`sudo apt-get install docker.io`

### Show downloaded Docker images
`docker image ls`

### Searching for remote Docker image (e.g. Redis):
`docker search redis`

### Downloading Docker image (e.g. Redis):
`docker pull redis`

### Starting up a container (e.g. Redis) with port binding:
`docker run -d --name redis_contner -p <PORT_OF_YOUR_CHOICE>:6379 redis`

or multiple binding:

`docker run -d -p 5801:5801 -p 5802:5802 ...`

### Listing containers:
`docker ps`

### Shutting down container:
`docker stop <container_id> -t 1`

### Accessing container terminal:
by ID:

`docker exec -i -t 665b4a1e17b6 /bin/bash`

by name:

`docker exec -i -t loving_heisenberg /bin/bash`
