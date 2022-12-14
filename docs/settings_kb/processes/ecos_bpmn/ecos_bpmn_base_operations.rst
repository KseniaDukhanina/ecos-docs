Базовые операции
================

.. _new_bp:

.. contents::

Создание
--------

Для создания нового бизнес-процесса необходимо перейти в левом меню в пункт **«Редактор бизнес-процессов»** или через верхнее меню **«Раздел администратора – Управление процессами – Модели бизнес-процессов»**.

 .. image:: _static/08.png
       :width: 300
       :align: center

Откроется форма создания карточки процесса:

 .. image:: _static/09.png
       :width: 600
       :align: center

.. list-table:: Описание полей формы
      :widths: 10 20 30
      :header-rows: 1
      :align: center
      :class: tight-table 

      * - п/п
        - Наименование
        - Описание
      * - 1
        - **Идентификатор**
        - уникальный идентификатор
      * - 2
        - **Имя**
        - наименование создаваемого бизнес-процесса
      * - 3
        - **Ecos Type**
        - тип данных. При привязке к типу данных можно автоматически начинать процесс, если проставлен  чекбокс **(7)**. На форме редактора на основе типа данных будут подтягиваться роли, статусы и т.д.
      * - 4
        - **Раздел**
        - наименование раздела, в котором будет сохранен процесс. Если не заполнять, то сохранение происходит в раздел "По умолчанию".
      * - 5
        - **Форма**
        - указать для запуска (старта) процесса через форму.
      * - 6
        - **Включен**
        - включение процесса
      * - 7
        - **Автоматический старт процесса**
        - при создании объекта указанного типа процесс будет запущен автоматически.

Сохранение и публикация
-----------------------

Процесс можно сохранить или сохранить о опубликовать.

 .. image:: _static/78.png
       :width: 600
       :align: center

Список процессов
----------------

.. list-table::
      :widths: 1 5
      :class: tight-table 

      * - 
               .. image:: _static/02.png
                :width: 50
                :align: center

        - представление в виде плитки|списка

Представление в виде списка:

 .. image:: _static/03.png
       :width: 600
       :align: center

Для редактирования процесса в редакторе нажмите:

 .. image:: _static/10.png
       :width: 600
       :align: center

Откроется :ref:`конструктор бизнес-процесса<modeller_bp>`

Карточка бизнес-процесса
------------------------

Для созданного процесса доступны следующие опции:

 .. image:: _static/04.png
       :width: 200
       :align: center

* **Просмотреть:**
  
        .. image:: _static/05.png
            :width: 600
            :align: center

*	**Удалить**
*	**Редактировать карточку процесса:**

        .. image:: _static/06.png
            :width: 600
            :align: center


*	**Редактировать бизнес-процесс:**

        .. image:: _static/07.png
            :width: 600
            :align: center


Способы запуска бизнес-процесса
---------------------------------

Существует два способа запуска бизнес-процесса:

1. Автоматический запуск БП при создании документа.

Осуществляется автоматически, если в описании БП указать необходимый **«Ecos Type»** и выставить флаг **«Автоматический старт процесса»** в положение истина.

2. Ручной запуск БП через форму

В описании БП в поле **«Форма»** можно указать форму запуска процесса, тогда ручной запуск осуществляется через **«Меню» -> «Создать» (+)**.

Способы автоматического старта и ручного запуска могут использовать как вместе, так и отдельно, в зависимости от бизнес требований.

В независимости от того, каким образом осуществляется старт бизнес-процесса, для возможности запуска, он должен быть «включен». 


Настройка меню
---------------

Для добавления процесса в меню **«Создать»**:

1.	Перейти в настройку меню, нажав на шестеренку, потом кнопку **«Настроить меню»** справа сверхуы.

 .. image:: _static/79.png
       :width: 600
       :align: center

2.	Выбрать элемент меню, в котором будет находиться процесс. Навести на элемент и нажать кнопку **«Добавить»**:

  .. image:: _static/80.png
        :width: 600
        :align: center

  - для описанного выше способа **1** выбрать **«Добавить ссылку на создание кейса»** из списка выбрать необходимый тип данных, нажать **«ОК»**:

  .. image:: _static/81a.png
        :width: 600
        :align: center

  - для описанного выше способа **2** выбрать **«Запустить бизнес-процесс»**, из списка выбрать необходимый процесс, нажать **«ОК»**.

 .. image:: _static/81b.png
       :width: 600
       :align: center

|

 .. image:: _static/82.png
       :width: 600
       :align: center

Добавленный пункт меню:

 .. image:: _static/83.png
       :width: 400
       :align: center


Форма запуска БП

 .. image:: _static/84.png
       :width: 600
       :align: center

Форма задачи БП

 .. image:: _static/85.png
       :width: 600
       :align: center