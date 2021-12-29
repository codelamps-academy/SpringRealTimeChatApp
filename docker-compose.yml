version: "3.6"

services:
  cassandra:
    container_name: cassandra
    image: cassandra:4.0
    ports:
      - 9160:9160
      - 9042:9042
      - 7199:7199
  redis:
    container_name: redis
    image: redis:6.2
    ports:
      - 6379:6379
  mysql:
    container_name: mysql
    image: mysql:8.0
    ports:
      - 3300:3306
    environment:
      - MYSQL_DATABASE=chat_app_databases
      - MYSQL_ROOT_PASSWORD=chat_app123
      - MYSQL_USER=chat_app
      - MYSQL_PASSWORD=chat_app1123
  rabbitmq:
    container_name: rabbitmq
    image: rabbitmq:alpine
    ports:
      - 15691:15691
      - 15692:15691
      - 25672:25672
      - 4369:4369
      - 5671:5671
      - 5672:5672
