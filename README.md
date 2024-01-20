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
![image](https://github.com/StepaBelyaev/Lab1/assets/70752929/1c8fbf94-00cb-41c1-98f6-a0f1960fb4b9)
Создадим собственный Realm: На боковой панели кликаем на Master - Create Realm - Задаем имя - Create.
![image](https://github.com/StepaBelyaev/Lab1/assets/70752929/44894183-afef-444e-9f7c-a0a6fe8cad74)
Создадим пользователей appadmin и user: На боковой панели кликаем на Users - Add User - Задаем необходимые значения - Create.
![image](https://github.com/StepaBelyaev/Lab1/assets/70752929/2c025d15-2507-487b-9dcc-669bc50bcd02)
![image](https://github.com/StepaBelyaev/Lab1/assets/70752929/ef7c0f75-b947-431c-9483-50d767b2262f)
![image](https://github.com/StepaBelyaev/Lab1/assets/70752929/0f404d7e-863d-4c82-b261-535c746c9e31)
Зададим им пароли: Users - Выбираем пользователя - Credentials - Задаем пароль.
![image](https://github.com/StepaBelyaev/Lab1/assets/70752929/4e3878ec-739d-477b-a920-94bced942ef3)
![image](https://github.com/StepaBelyaev/Lab1/assets/70752929/64c6b753-e583-4321-b894-644495845554)
Создадим клиента в Keycloack: На боковой панели кликаем на Clients - Creeate client - Задаем необходимые значения - Create.
![image](https://github.com/StepaBelyaev/Lab1/assets/70752929/859989e1-7daf-48c6-aa6f-db9fe1080786)
Создадим роли admin и user: На боковой панели кликаем на Clients - Выбираем нашего клиента - Roles - Create role - Задаем необходимые значения - Save.
![image](https://github.com/StepaBelyaev/Lab1/assets/70752929/a690813b-a250-4bcb-b935-de93d93bdc31)
# Шаг 3. Настройка Nextcloud
Настроим аутентификацию на Nextcloud: Скачаем в App "Social Login".
Затем перейдем в Административные настройки - Social Login - Custom Open ID Connet - Задаем необходимые параметры.
![image](https://github.com/StepaBelyaev/Lab1/assets/70752929/f030d728-66eb-4c4d-8f23-5d8d6931fa15)
Видим, что появилась ссылка на Keycloak
![image](https://github.com/StepaBelyaev/Lab1/assets/70752929/4b520163-3962-4b30-b8e8-ea562674ba54)
При нажатии она перенапрвляет на Keycloak
![image](https://github.com/StepaBelyaev/Lab1/assets/70752929/7066acb7-fbdb-442b-b0f6-e57d9f342588)
# Шаг 4. Настройка 2FA
В Keycloak переходим в Authentication - Browser - Browser Conditional OTP - Выбираем Required.
![image](https://github.com/StepaBelyaev/Lab1/assets/70752929/7863a0e1-4861-4c09-8828-cfb35a3b48b5)
Сканируем QR-код, прописываем данные
![image](https://github.com/StepaBelyaev/Lab1/assets/70752929/2e1b0375-c2b0-465e-8232-2c3addc2d33f)
Успешно попадаем на страницу
![image](https://github.com/StepaBelyaev/Lab1/assets/70752929/d7637915-0ac1-40f2-a14a-2239fcba9075)














