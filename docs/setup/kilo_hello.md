готов

1) Учебный сервис предварительной оценки заявки на заём под ПТС: принимает VIN, год, пробег, оценочную стоимость, сумму и срок, считает LTV и возвращает решение `approve` / `review` / `reject`. Все данные синтетические.

2) Makefile: `up`, `down`, `ps`, `logs`, `install`, `test`, `lint`, `seed`, `help`. docker-compose.yml: сервисы `backend` (Slim, порт 8080) и `db` (MySQL 8), healthcheck на `mysqladmin ping`, том `db-data`.

3) Решение `approve` / `review` / `reject` по заявке считается в `backend/src/Domain/DecisionEngine.php`.

модель: kilo/kilo-auto/free