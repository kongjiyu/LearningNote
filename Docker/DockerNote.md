# Docker Note
This note is used to make simple note for reference purpose in the future time

## To run docker for oracle
```cmd
docker run -d -p 1521:1521 -e ORACLE_PASSWORD=system -v oracle-volume:/u01/app/oracle/oradata gvenzl/oracle-xe
```

## To login
```cmd
sqlplus system/system@127.0.0.1
```

## To stop docker
```cmd
docker ps
```
Find the code of the docker container and
```cmd
docker stop {code}
```

## To delete docker container
```cmd
docker system prune -a
```