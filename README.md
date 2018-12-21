# docker-backing-services
Docker image description for the backing services (Redis, RabbitMQ)

## Prerequistes
1. Install Docker (https://docs.docker.com/install/#supported-platforms)
2. Clone the Repo
3. Run 'docker-compose' in terminal or command line

## Used Backing Services

1.  RabbitMQ for Messaging
2.  Redis as Cache for Key Value Pairs.

## VCAP SERVICES

VCAP_SERVICE for applications shall be used as environment variables.

```javascript
{
    "rabbitmq": {
        "hostname": "localhost",
        "password": "pass",
        "port": "5672",
        "uri": "amqp://rmq:pass@localhost:5672",
        "username": "rmq"
    },
    "redis": {
        "hostname": "localhost",
        "password": "pass1",
        "port": "6379"
    }
}
```
