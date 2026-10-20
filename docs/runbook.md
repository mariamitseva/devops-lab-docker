# Runbook

> Fill in every TODO with exact commands. / Попълнете всяко TODO с точни команди.

## Start locally / Локално стартиране

TODO

## Check that it works / Проверка, че работи

TODO: which address do you open and what should you see? / кой адрес отваряте и какво трябва да видите?

## Run the tests / Тестове

TODO

## When something breaks / Когато нещо се счупи

TODO: the first three things you check. / първите три неща, които проверявате.

## Стартиране с Docker

### 1. Build – изграждане на образа

```bash
docker build -t notes-api:0.3.0 .
```

Тази команда изгражда Docker образ с име `notes-api` и версия `0.3.0`.

### 2. Run – стартиране на контейнера

```bash
docker run -d --name notes-api-container -p 8000:8000 notes-api:0.3.0
```

Тази команда стартира приложението във фонов режим на порт 8000.

Приложението може да се провери на адрес `/health`.

### 3. Logs – преглед на логовете

```bash
docker logs notes-api-container
```

Показва съобщенията от работата на приложението.

### 4. Stop – спиране на контейнера

```bash
docker stop notes-api-container
```

Спира работещия контейнер.