# Проект YaMDb

![CI](https://github.com/BU-Marina/yamdb_final/actions/workflows/yamdb_workflow.yml/badge.svg?branch=master)

Собираются пользовательские отзывы на произведения по категориям (книги, фильмы и музыка).

## Шаблон наполнения env-файла

    DB_ENGINE=<engine>
    DB_NAME=<name>
    POSTGRES_USER=<username>
    POSTGRES_PASSWORD=<password>
    DB_HOST=<host>
    DB_PORT=<port>

    DEBUG=<debug>
    SECRET_KEY=''

## Запуск приложения в контейнерах

Выполнить из директории с файлом docker-compose.yaml

```
docker-compose up -d --build
```

## Заполнение БД начальными данными

```
docker-compose exec web python manage.py loaddata fixtures.json
```
