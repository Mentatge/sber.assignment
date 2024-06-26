# Shopping List Service

## Описание проекта

Shopping List Service представляет собой веб-приложение для управления списком покупок. Он предоставляет API для добавления, обновления, удаления и получения списка покупок пользователей.

## Структура проекта

Проект структурирован следующим образом:

- **Controller**: Контроллеры обрабатывают входящие HTTP-запросы и делегируют их обработку соответствующим сервисам.
- **DTO**: (Data Transfer Objects) используются для передачи данных между клиентом и сервером.
- **Entity**: Сущности представляют объекты, хранящиеся в базе данных, такие как продукты из списка покупок.
- **Repository**: Репозитории предоставляют методы для взаимодействия с базой данных.
- **Service**: Сервисы содержат бизнес-логику и выполняют операции над данными.
- **Exception**: Здесь обрабатываются исключения, возникающие в приложении.

## Используемые технологии

- **Java 17**: Язык программирования, используемый для разработки приложения.
- **Spring Boot**: Фреймворк для создания веб-приложений на основе Spring.
- **Spring Data JPA**: Инструмент для удобной работы с базой данных через Hibernate.
- **Lombok**: Библиотека для уменьшения шаблонного кода в Java-проектах.

## Инструкции по развертыванию

1. Убедитесь, что у вас установлены Java и Maven.
2. Склонируйте репозиторий на свой локальный компьютер.
3. Запустите приложение с помощью команды `mvn spring-boot:run`.
4. Проверьте работу API, обратившись к соответствующим эндпоинтам через любой клиент API.

## Эндпоинты

- **GET /getShoppingList**: Получение списка покупок пользователя.
- **POST /insertShoppingList**: Добавление элемента в список покупок.
- **DELETE /deleteShoppingList**: Удаление списка покупок.
- **PUT /updateShoppingList**: Обновление элемента в списке покупок.

## Обработка исключений

Исключения, возникающие во время выполнения, обрабатываются с помощью механизма `@ControllerAdvice`, который перехватывает и обрабатывает исключения глобально для всего приложения.

## Вклад

Этот проект разработан mentatge в рамках тестового задания для Сбер.

Если вы хотите внести вклад или исправить ошибку, пожалуйста, напишите мне или отправьте pull-request.

