FROM node:20.20.2-alpine3.23 AS builder
WORKDIR /app
COPY package.json .
COPY *.js .
RUN npm install


FROM node:20.20.2-alpine3.23 
WORKDIR /app
COPY --from=builder /app /app
ENV MONGO=true\
    MONGO_URL="mongodb://mongodb:27017/catalogue"
#RUN groupadd -r appgroup && useradd -r -g appgroup -m appuser
#USER appuser
ENTRYPOINT [ "node"]
CMD [ "server.js" ]












# FROM node:20
# WORKDIR /app
# COPY package.json .
# COPY *.js .
# RUN npm install
# ENV MONGO=true\
#     MONGO_URL="mongodb://mongodb:27017/catalogue"
# CMD [ "node", "server.js" ]
