FROM node:20
WORKDIR /app
#CMD [ "npm", "install" ]
ENV MONGO=true\
    MONGO_URL="mongodb://mongodb:27017/catalogue"
 COPY package.json .
 COPY *.js .
 RUN npm install