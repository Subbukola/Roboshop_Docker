FROM python:3
WORKDIR /app
COPY payment.ini .
COPY *.py .
COPY requirements.txt .
ENV CART_HOST=CART \
    CART_PORT=8080 \
    USER_HOST=user \
    USER_PORT=8080 \
    AMQP_HOST=rabbitmq \
    AMQP_USER=roboshop \
    AMQP_PASS=roboshop123
CMD [ "uwsgi", "--ini", "payment.ini" ]
