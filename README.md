## Run App

- Создать .env для окружения Laravel из .env.example
- cp src/.env.example src/.env
- ```docker compose build``` Собираем проект
- ```docker compose up -d``` Поднимаем контейнер
- ```docker compose exec php composer update``` Обновить композер
- ```docker compose exec php composer install``` Установить PHP библиотеки командной
- ```docker compose exec php php npm install```
- ```docker compose exec php chmod -R 777 storage``` Выдаём права на подключение к БД
- ```docker compose exec php php artisan key:generate``` Сгенерировать ключ приложения командной 
- ```docker compose exec php php artisan migrate:fresh --seed``` Создать таблицы и заполнить их данными
- http://localhost:8001 адрес доступа к приложению