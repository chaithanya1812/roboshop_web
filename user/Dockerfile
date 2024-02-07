FROM node:18-slim

WORKDIR  /app

RUN apt-get update && \
    apt-get install unzip -y

ADD https://roboshop-artifacts.s3.amazonaws.com/user.zip .

RUN unzip user.zip && \
    npm install

CMD ["node","./server.js"]



# NOTE :-
# IT's need's 3-Environment-variable so I am passing from Run-Time....
#   MONGO=true
#   MONGO="mongodb://<MONGODB-SERVER-IPADDRESS>:27017/catalogue"
#   REDIS_HOST=<REDIS-SERVER-IP>
