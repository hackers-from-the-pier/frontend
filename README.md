# Сервис уведомлений KiloWatt

Сервис для генерации PDF-уведомлений о подозрительной активности в энергопотреблении.

## Установка

1. Клонируйте репозиторий
2. Установите зависимости:

```bash
npm install
```

## Запуск

Для запуска в режиме разработки:

```bash
npm run dev
```

Для запуска в production режиме:

```bash
npm start
```

## API

### Получение PDF-уведомления

```
GET /v1/verify/notification-pdf/:id
```

Параметры:

- `id` - идентификатор уведомления

Ответ: PDF-файл с уведомлением

## Структура проекта

```
src/
  ├── controllers/
  │   └── notificationController.js
  ├── services/
  │   └── pdfGenerator.js
  └── server.js
```
