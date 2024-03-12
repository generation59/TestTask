# Тестовое задание: Flask приложение с выводом текущей даты и времени

## Описание
Этот проект представляет собой простое Flask приложение, которое выводит текущую дату и время. 
Приложение упаковано в контейнер с использованием Python 3.8 на базе Alpine Linux.

## Ссылка на экспортированный файл Docker образа

[https://cloud.mail.ru/public/Escv/Csbt6XWAn](https://cloud.mail.ru/public/Escv/Csbt6XWAn)

1. Импорт Docker образа
    ```bash
    docker load -i test.tar
    ```
2. Присваиваем тэг контейнеру
    ```bash
    docker tag <ID контейнера> test:latest
    ```
3. Запустите контейнер:
    ```bash
    docker run --name test --rm -p 5000:5000 test
    ```  


## Использование
Для запуска приложения необходимо выполнить следующие шаги:

1. Клонируем проект на компьютер.
    ```bash
    git@github.com:generation59/TestTask.git
    ```
2. Соберите Docker образ:
    ```bash
    docker build -t test .
    ```
3. Запустите контейнер:
    ```bash
    docker run --name test --rm -p 5000:5000 test
    ```
4. Проверьте работоспособность приложения:
    ```bash
    curl http://localhost:5000
    ```
