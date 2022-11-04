Создан контейнер для REST API сервера проекта из курса по Django (CRUD: Склады и запасы):

1. Обновлен файл requirements.txt
2. Сборка контейнера: docker build . --tag=my_stocks
3. Запуск: docker run -d -p 6060:6060 my_stocks
4. Для проверки работоспособности можно получить список продуктов (GET-запрос) здесь: http://localhost:8000/api/v1/products/, или отправить запрос из файла requests-examples.http.