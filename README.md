## CARA MENGHAPUS BANYAK DOCKER IMAGE
```
    docker rmi $(docker images -a -q)
```

## CARA MENGHAPUS BANYAK DOCKER CONTAINER
```
    docker stop $(docker ps -a -q)
    
    docker rm $(docker ps -a -q)
```

## CREATE DOCKER CONTAINER
# CASSANDRA
```
    docker run --rm \
    --name cassandra \
    -p 9042:9042 \
    cassandra:4.0
```

# REDIS
```
    docker run --rm \
    --name redisx \
    -p 6379:6379 \
    redis:6.2
```

# MYSQL
```
    docker run --rm \
    --name mysql_server \
    -e MYSQL_ROOT_PASSWORD=chat_app123 \
    -e MYSQL_DATABASE=ebook_chat_app \
    -p 3306:3306 \
    mysql:8.0
```