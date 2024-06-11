# 1 задание:

## CLICKHOUSE:
1. docker pull bitnami/clickhouse:latest

2. docker run --name clickhouse -p 8123:8123 -p 9000:9000 -e CLICKHOUSE_ADMIN_PASSWORD=12345 -d bitnami/clickhouse:latest

3. docker restart df1fa77d70ee5d9216f6908df5e1a9e0a72a3a86307932df0babc621414d88bd

4. docker stop df1fa77d70ee5d9216f6908df5e1a9e0a72a3a86307932df0babc621414d88bd

5. docker rm df1fa77d70ee5d9216f6908df5e1a9e0a72a3a86307932df0babc621414d88bd

6. docker run --name clickhouse_2 -p 8123:8123 -p 9000:9000 --cpus="1.5" --restart=unless-stopped -v /data/clickhouse:/var/lib/clickhouse -v /logs/clickhouse:/var/log/clickhouse-server -e CLICKHOUSE_ADMIN_PASSWORD=12345 -d bitnami/clickhouse:latest



## POSTGRES:
1. docker pull postgres:latest

2. docker run --name postgres_3 -e POSTGRES_USER=egor -e POSTGRES_PASSWORD=mysecretpassword -p 5400:5432 -d postgres

3. docker restart 2f1a9d7d2873debfead361b8078f7332773efa79c2ecd7fcfa8eff39ae246800

4. docker stop 2f1a9d7d2873debfead361b8078f7332773efa79c2ecd7fcfa8eff39ae246800

5. docker rm 2f1a9d7d2873debfead361b8078f7332773efa79c2ecd7fcfa8eff39ae246800

6. docker run --name postgres_3 -e POSTGRES_USER=egor -e POSTGRES_PASSWORD=mysecretpassword -p 5400:5432 --cpus="1.5" --restart=unless-stopped -v /path/on/host:/var/lib/postgresql/data -d postgres



# 2 задание, команды для поднятия docker-compose.yml:

1. cd %USERPROFILE%\Downloads

2. docker-compose up
