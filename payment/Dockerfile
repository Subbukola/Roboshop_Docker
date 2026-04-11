FROM python:3.9.25-alpine3.22 AS builder
WORKDIR /app
COPY payment.ini .
COPY *.py .
COPY requirements.txt .
RUN pip3 install -r requirements.txt


# FROM python:3.9.25-alpine3.22 
# WORKDIR /app
# COPY --from=builder /app /app

# RUN addgroup -S roboshop && adduser -S roboshop -G roboshop
# RUN chown -R roboshop:roboshop /app
# USER roboshop

# ENV CART_HOST=CART \
#     CART_PORT=8080 \
#     USER_HOST=user \
#     USER_PORT=8080 \
#     AMQP_HOST=rabbitmq \
#     AMQP_USER=roboshop \
#     AMQP_PASS=roboshop123
# CMD [ "uwsgi", "--ini", "payment.ini" ]














# FROM python:3
# WORKDIR /app
# COPY payment.ini .
# COPY *.py .
# COPY requirements.txt .
# RUN pip3 install -r requirements.txt
# ENV CART_HOST=CART \
#     CART_PORT=8080 \
#     USER_HOST=user \
#     USER_PORT=8080 \
#     AMQP_HOST=rabbitmq \
#     AMQP_USER=roboshop \
#     AMQP_PASS=roboshop123
# CMD [ "uwsgi", "--ini", "payment.ini" ]
