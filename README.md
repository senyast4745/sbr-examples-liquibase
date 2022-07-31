# Примеры кода для ШБР
Примеры кода из второй части лекции для Школы разработки бэкенда

## Темы
* Миграции. Liquibase

----
## Usage
1. Перед запуском тестов надо развернуть PostgreSQL. 
Можно сделать это в Docker с помощью команды:
```sh
docker run -e POSTGRES_PASSWORD=password -d -p 5432:5432 postgres
```
[Ссылка](https://hub.docker.com/_/postgres) на официальный образ PostgreSQL.

2. Накатить миграции
```sh
mvn liquibase:update
```
**!WARN!** Maven должен стоять на вашей машине
