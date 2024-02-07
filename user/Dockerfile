FROM node:18-slim

WORKDIR  /app

RUN apt-get update && \
    apt-get install unzip -y
ADD https://roboshop-artifacts.s3.amazonaws.com/cart.zip .

RUN unzip cart.zip && \
    npm install


CMD ["node","./server.js"]

#NOTE 3-Env
#Environment=REDIS_HOST=<REDIS-SERVER-IP>
#Environment=CATALOGUE_HOST=<CATALOGUE-SERVER-IP>
#Environment=CATALOGUE_PORT=8080

