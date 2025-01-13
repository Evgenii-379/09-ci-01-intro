# **Домашнее задание к занятию 7 «Жизненный цикл ПО»**-***Вуколов Евгений***
## **Подготовка к выполнению**
1. Получить бесплатную версию Jira - https://www.atlassian.com/ru/software/jira/work-management/free (скопируйте ссылку в адресную строку). Вы можете воспользоваться любым(в том числе бесплатным vpn сервисом) если сайт у вас недоступен. Кроме того вы можете скачать docker образ и запустить на своем хосте self-managed версию jira.
2. Настроить её для своей команды разработки.
3. Создать доски Kanban и Scrum.
4. Дополнительные инструкции от разработчика Jira.
## **Основная часть**
Необходимо создать собственные workflow для двух типов задач: bug и остальные типы задач. Задачи типа bug должны проходить жизненный цикл:

1. Open -> On reproduce.
2. On reproduce -> Open, Done reproduce.
3. Done reproduce -> On fix.
4. On fix -> On reproduce, Done fix.
5. Done fix -> On test.
6. On test -> On fix, Done.
7. Done -> Closed, Open.
Остальные задачи должны проходить по упрощённому workflow:

1. Open -> On develop.
2. On develop -> Open, Done develop.
3. Done develop -> On test.
4. On test -> On develop, Done.
5. Done -> Closed, Open.
## **Что нужно сделать**

1. Создайте задачу с типом bug, попытайтесь провести его по всему workflow до Done.
2. Создайте задачу с типом epic, к ней привяжите несколько задач с типом task, проведите их по всему workflow до Done.
3. При проведении обеих задач по статусам используйте kanban.
4. Верните задачи в статус Open.
5. Перейдите в Scrum, запланируйте новый спринт, состоящий из задач эпика и одного бага, стартуйте спринт, проведите задачи до состояния Closed. Закройте спринт.
6. Если всё отработалось в рамках ожидания — выгрузите схемы workflow для импорта в XML. Файлы с workflow и скриншоты workflow приложите к решению задания.
# **Как оформить решение задания**
Выполненное домашнее задание пришлите в виде ссылки на .md-файл в вашем репозитории.

## **Решение**

Схема рабочего процесса bug:
- ![scrin](https://github.com/Evgenii-379/09-ci-01-intro/blob/main/Снимок%20экрана%202025-01-11%20133155.png)

Перемещение задачи по доске kanban:
- ![scrin](https://github.com/Evgenii-379/09-ci-01-intro/blob/main/Снимок%20экрана%202025-01-12%20150809.png)
- ![scrin](https://github.com/Evgenii-379/09-ci-01-intro/blob/main/Снимок%20экрана%202025-01-12%20150823.png)
- ![scrin](https://github.com/Evgenii-379/09-ci-01-intro/blob/main/Снимок%20экрана%202025-01-12%20150903.png)
- ![scrin](https://github.com/Evgenii-379/09-ci-01-intro/blob/main/Снимок%20экрана%202025-01-12%20150924.png)
- ![scrin](https://github.com/Evgenii-379/09-ci-01-intro/blob/main/Снимок%20экрана%202025-01-12%20151023.png)

Задача epic связанная с другими задачами: 
- ![scrin](https://github.com/Evgenii-379/09-ci-01-intro/blob/main/Снимок%20экрана%202025-01-12%20151045.png)

Схема рабочего процесса epic:
- ![scrin](https://github.com/Evgenii-379/09-ci-01-intro/blob/main/Снимок%20экрана%202025-01-12%20161644.png)

- ![scrin](https://github.com/Evgenii-379/09-ci-01-intro/blob/main/Снимок%20экрана%202025-01-12%20161917.png)

Перемещение задачи по доске kanban:
- ![scrin](https://github.com/Evgenii-379/09-ci-01-intro/blob/main/Снимок%20экрана%202025-01-12%20224650.png)
- ![scrin](https://github.com/Evgenii-379/09-ci-01-intro/blob/main/Снимок%20экрана%202025-01-12%20224713.png)
- ![scrin](https://github.com/Evgenii-379/09-ci-01-intro/blob/main/Снимок%20экрана%202025-01-12%20224821.png)
- ![scrin](https://github.com/Evgenii-379/09-ci-01-intro/blob/main/Снимок%20экрана%202025-01-12%20225041.png)

Доска scrum:
- ![scrin](https://github.com/Evgenii-379/09-ci-01-intro/blob/main/Снимок%20экрана%202025-01-13%20142430.png)
- ![scrin](https://github.com/Evgenii-379/09-ci-01-intro/blob/main/Снимок%20экрана%202025-01-13%20144959.png)

- [bug](xml/workflow_bug.xml)
- [task](xml/workflow_task.xml)













