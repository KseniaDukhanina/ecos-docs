.. _service_develop:

Разработка микросервисов
==========================

В данной статье пойдет речь о разработке следующих микросервисов:

- ecos-gateway;
- ecos-model;
- ecos-uiserv;
- ecos-process;
- ecos-apps;
- ecos-notifications;
- ecos-history.

Требования
--------------

- JDK 8
- Maven версии 3.0.0 или выше

Все микросервисы из списка выше построены на основе тех же технологий, на основе которых создается новый микросервис :ref:`в статье<service_setup>`

Команды для работы с микросервисами
------------------------------------

Выполнение тестов:

.. code-block::

    mvn clean test


Запуск микросервиса для локальной разработки:

.. code-block::

    mvn spring-boot:run

Вместо этой команды можно использовать возможности IDE для запуска spring-boot приложений.

Сборка docker образа:

.. code-block::

    mvn clean package jib:dockerBuild -Djib.docker.image.tag=1.0.0-snapshot

где,

**1.0.0-snapshot** - это версия микросервиса, которая будет тэгом нашего образа

При сборке образ попадет в локальный реестр docker и его можно будет использовать в docker-compose файлах.

