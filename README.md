# Домашнее задание к занятию "`Обзор систем IT-мониторинга`" - `Викулов Александр`

### Задание 1

`Процесс выполнения`

1. `Открываем облачную платформу Yandex.Cloud`

    <kbd>  
      <img src="https://github.com/AleksandrVikulov/08-01-monitoring-systems/raw/main/task_img/01.png">
    </kbd>

2. `Создаем виртуальную машину с конфигурацией согласно заданию:`
    * `ОС:          Debain 11`
    * `HDD:         3GB`
    * `Платформа:   Intel Ice Lake`
    * `vCPU:        2`
    * `доля vCPU:   20%`
    * `RAM:         1GB`
    * `Прерываемая: да`

    <kbd>  
      <img src="https://github.com/AleksandrVikulov/08-01-monitoring-systems/raw/main/task_img/02-1.png">
    </kbd>
    <kbd>  
      <img src="https://github.com/AleksandrVikulov/08-01-monitoring-systems/raw/main/task_img/02-2.png">
    </kbd>ng)

3. `Создаем сервисный аккаунт с ролью monitoring.editor`

    ![Image alt](https://github.com/AleksandrVikulov/08-01-monitoring-systems/raw/main/task_img/03.png)

4. `Сгенерируем SSH-ключ`

    ![Image alt](https://github.com/AleksandrVikulov/08-01-monitoring-systems/raw/main/task_img/04.png)

5. `Настроим доступ к ВМ, указав сервисный аккаунт с ролью monitoring.editor, логин и сгенерированный SSH-ключ`

    ![Image alt](https://github.com/AleksandrVikulov/08-01-monitoring-systems/raw/main/task_img/05.png)
    
6. `Устанавливаем агент сбора метрик`

    ![Image alt](https://github.com/AleksandrVikulov/08-01-monitoring-systems/raw/main/task_img/06.png)

7. `Создаем ВМ с нужными параметрами`

    ![Image alt](https://github.com/AleksandrVikulov/08-01-monitoring-systems/raw/main/task_img/07.png)

8. `Переходим в серсим мониторинга, создаем Дашборд, добавляем на него график и создаем параметры запросы для графика`

    ![Image alt](https://github.com/AleksandrVikulov/08-01-monitoring-systems/raw/main/task_img/08.png)

9. `Установим время сейчас и увидим график по выбранному запросу`

    ![Image alt](https://github.com/AleksandrVikulov/08-01-monitoring-systems/raw/main/task_img/09.png)

10. `Выходим и сохраняем дашборд`

    ![Image alt](https://github.com/AleksandrVikulov/08-01-monitoring-systems/raw/main/task_img/10.png)

---
## Дополнительные задания (со звездочкой*)

Эти задания дополнительные (не обязательные к выполнению) и никак не повлияют на получение вами зачета по этому домашнему заданию. Вы можете их выполнить, если хотите глубже и/или шире разобраться в материале.

### Задание 2

1. `Вернемся на основную вкладку мониторинга и в том же месте, где нажимали создать дашборд, нажмем создать алерт.`
2. `Введем название алерта`

   ![Image alt](https://github.com/AleksandrVikulov/08-01-monitoring-systems/raw/main/task_img/11.png)

3. `Настроим основные метрики: укажем для какой машины применяются метрики, укажем параметры загрузки процессора - выше 50% предупреждение, выше 75% аларм`

   ![Image alt](https://github.com/AleksandrVikulov/08-01-monitoring-systems/raw/main/task_img/12.png)

4. `Создадим почтовый канал для уведомлений`

   ![Image alt](https://github.com/AleksandrVikulov/08-01-monitoring-systems/raw/main/task_img/13.png)
   ![Image alt](https://github.com/AleksandrVikulov/08-01-monitoring-systems/raw/main/task_img/14.png)

5. `Создаем и сохраняем алерт, и получаем возможность следить за его статусом их интерфейса мониторинга`

   ![Image alt](https://github.com/AleksandrVikulov/08-01-monitoring-systems/raw/main/task_img/15.png)

