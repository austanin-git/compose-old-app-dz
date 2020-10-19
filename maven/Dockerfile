FROM maven:alpine

# Pull github project

WORKDIR /app/
RUN apk update git;\
    apk add --no-cache git ;\
    git clone https://github.com/austanin-git/compose-old-app

# Changing working directory

WORKDIR /app/compose-old-app

RUN cp /app/compose-old-app/WebContent/Config.propeties /app/compose-old-app/Config.propeties

# Maven package

RUN mvn install
