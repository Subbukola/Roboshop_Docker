FROM node:20
WORKDIR /app
ENV MONGO=true\
    MONGO_URL="mongodb://mongodb:27017/catalogue"
 COPY package.json .
 COPY *.js .
 #RUN npm install
 CMD [ "npm", "install" ]
