# cmd when Creating database
```
## put dump on ./tmp
## first, enter in docker container
docker-compose exec db bash

## second, import dump
sh-5.1# psql -d postgres -U postgres -c "create database dev WITH ENCODING='UNICODE' owner=postgres"

#CREATE DATABASE
bash-5.1# psql -d postgres -U postgres -f /tmp/postgresdb.dump
```
