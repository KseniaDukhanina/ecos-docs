Событийный подпроцесс
=====================

.. _event_subprocess:

**Событийный подпроцесс** - подпроцесс, запускаемый событием.

Событийный подпроцесс изображается на схеме прямоугольником с закругленными углами и границей, выполненной тонкой пунктирной линией.

 .. image:: _static/bpmn_start_event_sub_process_overview.png
       :width: 500
       :align: center

Для создания событийного подпроцесса создайте сначала стандартный :ref:`подпроцесс<sub_process>`. И далее выберите:

 .. image:: _static/bpmn_start_event_sub_process_new.png
       :width: 400
       :align: center

Событийный подпроцесс BPMN запускается собственным стартовым событием и не имеет входящих и исходящих потоков операций, что отличает его от обычного подпроцесса, который запускается потоком операций родительского процесса.

Для запуска событийного подпроцесса могут быть использованы следующие типы событий:

    -	:ref:`Таймер<ecos_bpmn_timer>`;
    - :ref:`Событие Citeck<ecos_bpmn_events>`.

 .. image:: _static/bpmn_start_event_sub_process_new_elements.png
       :width: 300
       :align: center

Событийный подпроцесс может быть **прерывающим (interrupting)** и **непрерывающим (non-interrupting)**.

    -	**Прерывающий** событийный подпроцесс. При его запуске процесс верхнего уровня приостановил выполнение (например, нужно разобраться с поступившей новой информацией, а после этого вышестоящий процесс может и вообще не потребоваться). При этом в одно время может работать только один экземпляр прерывающего событийного подпроцесса.
    -	**Непрерывающий** событийный подпроцесc.  Не прерывает основной процесс и выполняется параллельно с ним. Например, параллельно с работой основного процесса может идти его проверка или иное действие. Непрерывающих событийных процессов может одновременно выполняться несколько.

Прерывающий и непрерывающий событийные подпроцессы отличаются друг от друга только типом стартового события, поэтому настройка этого отличия производится не из свойств подпроцесса, а из свойств стартового события:

 .. image:: _static/bpmn_start_event_sub_process_start_element.png
       :width: 300
       :align: center

**1** – стартовые события для **прерывающего** событийного подпроцесса

**2** – стартовые события для **непрерывающего** событийного подпроцесса

Создание остальных элементов подпроцесса аналогично описанным в разделе :ref:`Компоненты Citeck BPMN<ecos_bpmn_components>`.

