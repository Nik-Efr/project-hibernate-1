1. Проект: Работа с Hibernate ORM
   Проект для изучения и демонстрации возможностей Hibernate ORM.
   Включает настройку базы данных, создание сущностей, работу с сессиями и выполнение CRUD операций.

2. Собрать и запустить
   mvn clean package
   docker run --name mysql-rpg -e MYSQL_ROOT_PASSWORD=root -e MYSQL_DATABASE=rpg -p 3306:3306 -d mysql:8.0
   Проинициализировать базу данных с помощью resources/init.sql
   Поднять на Tomcat 10 (artifact war exploded)

3. Технические особенности
   Настроена конфигурация Hibernate через PlayerRepositoryDB
   Реализованы маппинги сущностей с использованием аннотаций JPA
   Использован паттерн DAO для работы с данными

4. Функциональность
   Создание и настройка SessionFactory
   CRUD операции
   Работа с транзакциями
