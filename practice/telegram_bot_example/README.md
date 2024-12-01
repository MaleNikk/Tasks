Приложение для телеграм бота.
 
 Основные моменты настройки:

1. Открыть проект в среде разработки.
2. Открыть терминал, перейти в директорию: cd docker, выполнить: docker compose up.
3. Запустить телеграм.
4. Создать и войти в телеграм бот.
5. Запустить приложение.
6. Ввести команду start.
7. Использовать по назначению.

 Настройки приложения в application.yaml:
 binance.api.getPrice - источник информации о стоимости криптовалют
 time.upload.fixed - время отправки сообщений пользователю:
 (метод рассчитывает разницу между зафиксированной стоимостью и текущей)
 telegram.connection:
 username: - имя бота пользователя
 token: - токен пользователя
 
Особенности приложения:
 - нет возможности реализовать несколько обработчиков команд как для одного,
   так и для разных пользователей.
 - в базе данных может быть только одна сущность с сохраненной стоимостью криптовалюты.
 - возможность расширять функционал приложения с разными логическими операциями.
 - в основе хранилища данных - mongodb.