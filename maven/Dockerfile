FROM maven:alpine

# Pull github project

WORKDIR /app/
RUN apk update git;\
    apk add --no-cache git ;\
    git clone https://github.com/austanin-git/compose-old-app

# Changing working directory

WORKDIR /app/compose-old-app

# Maven package

RUN mvn install
