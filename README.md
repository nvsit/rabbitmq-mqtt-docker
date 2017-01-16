# rabbitmq-mqtt-docker
RabbitMQ Dockerfile with default configuration to run MQTT Broker

# Run 
```
$ docker build -t rmq-mqtt .

$ docker run -it \
    -p 15672:15672 -p 5672:5672 -p 1883:1883 \
    -v $PWD/docker/var/lib/rabbitmq:/var/lib/rabbitmq \
    rmq-mqtt
```
