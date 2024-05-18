# Домашнее задание к занятию «Система мониторинга Zabbix» - «Почикаев Василий»

В
### Задание 1 

Установите Zabbix Server с веб-интерфейсом.

#### Процесс выполнения
1. Выполняя ДЗ, сверяйтесь с процессом отражённым в записи лекции.
2. Установите PostgreSQL. Для установки достаточна та версия, что есть в системном репозитороии Debian 11.
3. Пользуясь конфигуратором команд с официального сайта, составьте набор команд для установки последней версии Zabbix с поддержкой PostgreSQL и Apache.
4. Выполните все необходимые команды для установки Zabbix Server и Zabbix Web Server.

#### Требования к результаты 
1. Прикрепите в файл README.md скриншот авторизации в админке.
2. Приложите в файл README.md текст использованных команд в GitHub.

---
### Решение 

![z](https://github.com/PochikaevVV/HW_netology/blob/main/img/z1_1.png)

'
pvv@REMBO MINGW64 ~
$ cd zabbix-part1/

pvv@REMBO MINGW64 ~/zabbix-part1 (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   zabbix-part1.md

no changes added to commit (use "git add" and/or "git commit -a")

pvv@REMBO MINGW64 ~/zabbix-part1 (main)
$ git add *

pvv@REMBO MINGW64 ~/zabbix-part1 (main)
$ git commit -a "z1"
fatal: paths 'z1 ...' with -a does not make sense

pvv@REMBO MINGW64 ~/zabbix-part1 (main)
$ git commit -m "z1"
[main f3507e5] z1
 1 file changed, 57 insertions(+)

pvv@REMBO MINGW64 ~/zabbix-part1 (main)
$ git push origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 1.42 KiB | 1.42 MiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/PochikaevVV/HW_netology.git
   0b97869..f3507e5  main -> main

pvv@REMBO MINGW64 ~/zabbix-part1 (main)
$ mkdir img

pvv@REMBO MINGW64 ~/zabbix-part1 (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

pvv@REMBO MINGW64 ~/zabbix-part1 (main)
$ git add *

pvv@REMBO MINGW64 ~/zabbix-part1 (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

pvv@REMBO MINGW64 ~/zabbix-part1 (main)
$ git init
Reinitialized existing Git repository in C:/Users/pvv/zabbix-part1/.git/

pvv@REMBO MINGW64 ~/zabbix-part1 (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        img/

nothing added to commit but untracked files present (use "git add" to track)

pvv@REMBO MINGW64 ~/zabbix-part1 (main)
$ git add *

pvv@REMBO MINGW64 ~/zabbix-part1 (main)
$ git commit -m "z1"
[main 43b1e62] z1
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 img/z1_1.png

pvv@REMBO MINGW64 ~/zabbix-part1 (main)
$ git push origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (4/4), 22.36 KiB | 22.36 MiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/PochikaevVV/HW_netology.git
   f3507e5..43b1e62  main -> main

pvv@REMBO MINGW64 ~/zabbix-part1 (main)

'

### Задание 2 

Установите Zabbix Agent на два хоста.

#### Процесс выполнения
1. Выполняя ДЗ, сверяйтесь с процессом отражённым в записи лекции.
2. Установите Zabbix Agent на 2 вирт.машины, одной из них может быть ваш Zabbix Server.
3. Добавьте Zabbix Server в список разрешенных серверов ваших Zabbix Agentов.
4. Добавьте Zabbix Agentов в раздел Configuration > Hosts вашего Zabbix Servera.
5. Проверьте, что в разделе Latest Data начали появляться данные с добавленных агентов.

#### Требования к результаты 
1. Приложите в файл README.md скриншот раздела Configuration > Hosts, где видно, что агенты подключены к серверу
2. Приложите в файл README.md скриншот лога zabbix agent, где видно, что он работает с сервером
3. Приложите в файл README.md скриншот раздела Monitoring > Latest data для обоих хостов, где видны поступающие от агентов данные.
4. Приложите в файл README.md текст использованных команд в GitHub

---
### Решение 

## Задание 3 со звёздочкой*
Установите Zabbix Agent на Windows (компьютер) и подключите его к серверу Zabbix.

#### Требования к результаты 
1. Приложите в файл README.md скриншот раздела Latest Data, где видно свободное место на диске C:
--- 

## Критерии оценки

1. Выполнено минимум 2 обязательных задания
2. Прикреплены требуемые скриншоты и тексты 
3. Задание оформлено в шаблоне с решением и опубликовано на GitHub



