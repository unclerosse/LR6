# LR6
Лабораторная работа №6

## Цель работы
Изучение базовых возможностей системы управления версиями, опыт работы с Git Api, опыт работы с локальным и удаленным репозиторием.

## Ход работы
1. Создали аккаунт на GitHub. [Рисунок 1](/images/1.jpg)
2. Сделали копию в личное хранилище из удалённого репозитория.
3. Установили Git.
4. После установки настроить клиент git, введя имя пользователя и email. [Рисунок 2](/images/2.jpg)
5. Клонировали свой личный удалённый репозиторий на компьютер.
6. Добавили файл через интерфейс GitHub. Подтянули изменения в локальный репозиторий. [Рисунок 3](/images/3.png)
7. Получили историю операций для каждой из веток. [Рисунок 4](/images/4.png) [Рисунок 5](/images/5.png)
8. Посмотрели последние изменения. [Рисунок 6](/images/6.png)
9. Выполнили слияние в ветку master, разрешив конфликт. [Рисунок 7.1](/images/7.png) [Рисунок 7.2](/images/merge.png)
10. Удалили побочную ветку после успешного слияния. [Рисунок 8](/images/8.png)
11. Сделали изменения и зафиксировать их, оставляя комментарии, несколько раз. [Рисунок 9](/images/9.png)
12. Сделали откат коммита. [Рисунок 10](/images/10.png)
13. Создали ветку для отчёта. [Рисунок 11](/images/11.png)
14. Начали оформлять отчёт в файле README.md, используя markdown синтаксис
15. Получили историю операций в форматированном виде. [Рисунок 12](/images/12.png)
16. Отправили локальные изменения в сетевое хранилище GitHub.

### История операций в форматированном виде
dda8ad2 - Wed Nov 15 23:46:09 2023 +0300 | 4125 gleb besedin | добавил пункты 6-9 отчёта, добавил все скриншоты выполнения комманд
935f7d0 - Wed Nov 15 23:45:09 2023 +0300 | 4125 gleb besedin | добавил пункты 1-5 отчёта, добавил скриншоты выполнения комманд
78d9bb3 - Wed Nov 15 23:12:45 2023 +0300 | 4125 gleb besedin | исправил mergefile.txt
5513ed1 - Wed Nov 15 22:56:43 2023 +0300 | gleb betelgeuse | Create file.txt
921f53b - Sat Nov 21 20:09:49 2020 +0300 | Kurtyanik | Обновление информации
0f9f50d - Sat Nov 21 20:08:33 2020 +0300 | Kurtyanik | Заполнил файл
c08a654 - Sat Nov 21 20:02:16 2020 +0300 | Kurtyanik | Файл создан пустым
3c6e913 - Sat Nov 21 19:58:20 2020 +0300 | Kurtyanik | Initial commit

## Лог комманд
`git clone https://github.com/unclerosse/LR6.git lw6`
`git config user.name; git config user.email`
`git pull origin master`
`git log`
`git checkout branch1`
`git log`
`git checkout master`
`git diff master..branch1`
`git merge branch1`
`git status`
`git add .\mergefile.txt`
`git status`
`git commit -m 'исправил mergefile.txt'`
`git branch -d branch1`
`git add .`
`git commit -m "Добавил АБСОЛЮТНО НОВЫЙ ФАЙЛ"`
`git reset --hard HEAD^`
`git push`
`git checkout -b report`
`git add .\README.md`
`git add .\images\*.jpg`
`git commit -m 'добавил пункты 1-5 отчёта, добавил скриншоты выполнения комманд'`
`git add .\README.md`
`git add .\images\.`
`git commit -m 'добавил пункты 6-9 отчёта, добавил все скриншоты выполнения комманд'`
`git log --pretty=format:"%h - %ad | %an | %s"`
`git add .\README.md`
`git add .\images\12.png`
`git commit -m 'добавил пункты 10-15 отчёта, добавил новый скриншот'`
