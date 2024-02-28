# tinyurl
REST API web service written in Spring-Boot (Java), allows users to short URLs, monitor, track after them, and see statistics.

# Tools
### Databases:
- Redis: Mapping the long URL to a short one.
- MongoDB: For users management.
- Cassandra: For clicks statistics.
### Container
- Docker


## How To Run
1. Clone the project
```
git clone git@github.com:roee-tal/tiny-url.git
```
3. Go to the project directory - use docker compose (make sure you have docker installed)
```
docker-compose up -d
```
4. To create cassandra key space you may need to run this command before on the cassandra machine
```
CREATE KEYSPACE tiny_keyspace
WITH replication = {'class':'SimpleStrategy', 'replication_factor' : 1};
```
5. After starting the server you can use the swagger on this adress:
```
http://localhost:8080/swagger-ui.html#
```

Enjoy!


