FROM node:18-slim

WORKDIR  /app

ADD https://roboshop-artifacts.s3.amazonaws.com/catalogue.zip .

RUN apt-get update && \
    apt-get install unzip -y && \
    unzip catalogue.zip && \
    npm install

CMD ["node","./server.js"]
LABEL projectName=roboShop \
      env=dev

# NOTE :-
# IT's need's 2-Environment-variable so I am passing from Run-Time....
#   MONGO=true
#   MONGO="mongodb://<MONGODB-SERVER-IPADDRESS>:27017/catalogue"
