# Docker

![docker](Moby-logo.png)

---

## Docker Command

> Docker pull command

```

docker container run --publish 80:80 --detach --name  webserver nginx

docker container run -d -p 3306:3306 --name db -e MYSQL_RANDOM_ROOT_PASSWORD=yes mysql

```

> Docker Useful commands

```
   docker inspect

   docker stats
```

> list all running container

```
docker container ls
```

> list all container

```
docker container ls -a
```

> Docker for running os and get inside

```
docker container run -it --name ubuntu4 ubuntu
```

> Docker run Existing Local Image

```
docker container run -ai ubuntu
```

> Docker get inside container by bash

```
docker container run -it --name webngix nginx  bash
```

> Start container

```
docker container start  -ai  ubuntu
```

```
docker container exec -it mysql bash
```

> Docker build 
```
  docker build -t flask_app . | name & current directory 

  ```
> Docker image Name 
```
docker image tag html-nginx2  najaah88/html_nginx:v1
```
> Run Custom image 
```
docker container run -p 80:80 --rm html-nginx2

```
> Docker push 
```
docker push najaah88/html_nginx:v1 
```

---

# Docker network

```
docker network ls
docker network create my_network
docker container run -d -p 8000:80 --name nginexx -network my_network nginx



```

> Connect a Network

```
docker network  connect my_network| networkID  containerID|nginnexx
```

> Disconnect a Network

```
docker network  disconnect my_network| networkID  containerID|nginnexx
```

---

> BY: Najah Said
