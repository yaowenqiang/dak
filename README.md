Docker and Kubernetes the compelte guide

> docker run -it redis
> docker version | grep os
> docker run busybox echo hi there

docker run = docker create + docker start

> docker crreate hello-world
> docker start -a containerID
> docker start containerID
> docker system prune
> docker stop containerID SIGTERM 10s 
> docker kill containerID SIGKILL
> docker exec -it containerID redis-cli
> docker exec -it containerID sh
> docker run -it busybox sh


Rebuild with Cache

> docker build  -t yaowenqiang/redis:last .
> docker commit -c "CMD ["redi-server"]"  containerID 



docker-compose

> docker-compose up
> docker-compose up --build
> docker-compose up -d
> docker-compose down
> docker-compose ps

automitic restart crashed container

restart Policies

+ "no"  Never attempt to restart this container if it stops or crashes no will be parsed as false without quote
+ always If this container stops "for any reason" always attempt to restart it
+ on-failure Only restart if the container stops with an error code
+ unless-stopped  Always restart unless we (the developers) forcebly stop it

> docker-compose top



