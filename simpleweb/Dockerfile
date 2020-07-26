FROM node:alpine
RUN sed -i 's/dl-cdn.alpinelinux.org/mirrors.aliyun.com/g' /etc/apk/repositories
WORKDIR /usr/app
#COPY ./ ./
COPY ./package.json  ./
RUN npm install
COPY ./ ./


CMD ["npm","start"]
