## Build it

`docker build -t bs/rabbitmq:latest .`

## Run it

```
docker run --name="rabbitmq" \
  -p 5672:5672 \
  -p 15672:15672 \
  -p 61613:61613  \
  -e RABBITMQ_USER=$RABBITMQ_USER \
  -e RABBITMQ_PASS=$RABBITMQ_PASS \
  bs/rabbitmq:latest
```
