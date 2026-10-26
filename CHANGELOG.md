# Changelog

## Unreleased

## 0.4.0 - 2026-10-26

- Добавено стартиране на Notes API и PostgreSQL чрез Docker Compose.
- Зададена версия на приложението APP_VERSION=0.4.0.
- Добавен именуван volume за запазване на бележките.
- Добавени healthcheck за PostgreSQL и изчакване чрез service_healthy.
- Добавен .env.example; .env е изключен от Git и Docker образа.
- Добавен Adminer с профил tools.
- Допълнен runbook с инструкции за Compose.
- Прието ADR 0002 за използване на PostgreSQL.

## Initial template

- Initial template: notes API with health and version endpoints.
