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




