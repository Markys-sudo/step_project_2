# Step Project 2 - Upload Server

Проект предназначен для запуска сервера загрузки изображений с использованием Docker, PostgreSQL и PgBouncer.

## Структура проекта
```
.
├── services
│ ├── backend # Python-сервис для загрузки изображений
│ ├── pgbouncer # Конфигурация PgBouncer
│ └── nginx # Конфигурация Nginx
├── init-sql # Скрипты инициализации базы PostgreSQL
├── images # Папка для хранения загруженных изображений
├── logs # Логи приложения и Nginx
├── docker-compose.yml
├── .env.sample
└── requirements.txt
```

## Запуск проекта

1. Скопируйте `.env.sample` в `.env` и заполните переменные окружения.
2. Соберите и запустите контейнеры:

```bash
docker-compose up --build 
```

