# Docker

## The Case for Docker
* Accelerate Devloper Onboarding
* Eliminate App Conflicts
* Environment Consistency
* Ship Software Faster

## Understand Dockerfiles
* Dockerfile => docker build => Docker Image
```
FROM node:alpine
LABEL author="Codewizz"
ENV NODE_ENV=production
WORKDIR /var/www
COPY . .
RUN npm install
EXPOSE 3000
ENTRYPOINT ["node", "server.js"]
```

## Using docker build
* `docker build -t <image name> .`
* `docker build -t <registry>/<name>:<tag> .`
	* docker build -t cckcoder/fastapi:1.0 .
