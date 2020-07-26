# Use an existing docker image as a base
FROM alpine
RUN sed -i 's/dl-cdn.alpinelinux.org/mirrors.aliyun.com/g' /etc/apk/repositories
# Download and install a dependency
RUN apk add --update redis

# Tell the image what to do when it starts

# as a container

CMD [ "redis-server" ]
