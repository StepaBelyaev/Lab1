## Отчет по Лабораторной работе №1

# Шаг 1. Начальная настройка
На первой ВМ запустим Keycloack с помощью Docker
![image](https://github.com/StepaBelyaev/Lab1/assets/70752929/69c8bed8-35de-4dcd-871a-e44aeccbfbe0)
На второй ВМ запсутим Nextcloud с помощью Docker-compose
![image](https://github.com/StepaBelyaev/Lab1/assets/70752929/c804c68f-14d2-485e-bba1-66e24ca2fa28)

# Шаг 2. Настроим сервер Keycloack
В браузере переходимна на веб-интерфейс KeyCloak
![image](https://github.com/StepaBelyaev/Lab1/assets/70752929/b346f97d-e4bd-48c9-9934-1045ee1adbeb)
Затем переходим в Administrative console с помощью учетных данных, используемых при запуске контейнера.
Создадим собственный Realm: На боковой панели кликаем на Master - Create Realm - Задаем имя - Save.
