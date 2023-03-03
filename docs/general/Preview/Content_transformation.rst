.. _content_transformation:

Трансформация содержимого документов
=====================================

.. note::

    Доступно только в enterprise версии.

Трансформации выполняются в микросервисе :ref:`ecos-transformations <transformation>`. 

Настройки трансформации:

.. code-block:: 

    ecos:
    webapp:
        task:
        executors:
            transformations:
            corePoolSize: 10 # количество потоков трансформации

**Конвертация** - частный случай трансформации, который подразумевает изменение содержимого из одного формата в другой. 

Для конвертации между типами документов используется OnlyOffice.

OnlyOffice
------------

Настройки:

.. code-block:: 

    ecos:
    integrations:
        onlyoffice:
        host: only-office-app # хост, на котором доступен сервер OnlyOffice
        port: 80 # http порт для работы с OnlyOffice

Типы трансформаций
-------------------

  .. list-table::
        :widths: 10 50 50
        :header-rows: 1
        :class: tight-table 

        * - Идентификатор
          - Конфигурация
          - Описание
        * - **convert**
          - | **converter: String** // идентификатор конкретного конвертера. Если не задан, то вычисляется автоматически
            | **toMimeType: String** // MIME type, содержимого, которое мы хотим получить по итогу конвертации
          - Конвертирование содержимого из одного MIME type в другой.
        * - **barcode**
          - | 
          - Добавление баркода на документ