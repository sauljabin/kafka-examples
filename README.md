# cp-kafka-docker

Example of kafka cluster using the official image. Thi is for development purpose.

## Documentation

- [Kafka](https://hub.docker.com/r/confluentinc/cp-kafka)
- [Zookeeper](https://hub.docker.com/r/confluentinc/cp-zookeeper)
- [Confluent](https://docs.confluent.io/platform/current/installation/docker/config-reference.html)

## Getting Started

```
$ make up
```

## Default Ports

| Port | Description |
| - | - |
| 12181 | Zookeeper port |
| 19093 | Kafka port |

## Docker Stack Examples

- [docker-compose.yml](docker-compose.yml)

## Make Commands

#### Builds the docker image
```
$ make build
```

#### Deploys a kafka broker
```
$ make up
```

#### Shows the stack status
```
$ make status
```

#### Stops stack
```
$ make down
```

#### Opens a terminal inside kafka
```
$ make bash-kafka[123]
```

#### Opens a terminal inside zookeeper
```
$ make bash-zookeeper[123]
```

#### Shows kafka's logs
```
$ make log-kafka[123]
```

#### Shows zookeeper's logs
```
$ make log-zookeeper[123]
```

## Commands for Kafka

#### Creates a topic
```
$ make create-topic topic=test
```

#### Shows the topic list
```
$ make topic-list
```

#### Creates a console producer connection
```
$ make producer topic=test
```

#### Creates a console consumer connection
```
$ make consumer topic=test
```

#### Describes a topic
```
$ make describe topic=test
```
