# Real_Time
1. Open docker
2. Open CMD in working folder directory and run code
```sh
$ docker-compose up
```
3. Once the services are running, open another tab and pre-create the Kafka topic


Note
- To access postgreSQL in docker terminal
```sh
$ psql -U <dataBaseUserName> <dataBaseName>
```
```sh
$ psql -U root root
```
- To 

-docker-compose exec elasticsearch curl -XGET "localhost:9200/topic1/_search?format=json&pretty"
- docker-compose exec kafka kafka-topics \
    --bootstrap-server localhost:9092 \
    --topic topic1 \
    --replication-factor 1 \
    --partitions 4 \
    --create
