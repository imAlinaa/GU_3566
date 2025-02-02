# Инструкция для работы с Git и удалёнными репозиториями

## Что такое Git?
Git - это одна из реализаций распределённых систем контроля версий, имеющая как и локальные, так и удалённые репозитории. Является самой популярной реализацией систем контроля версий в мире.
## Подготовка репозитория
Для создание репозитория необходимо выполнить команду *git init*  в папке с репозиторием и у Вас создаться репозиторий (появится скрытая папка .git)

## Создание коммитов

### Git add
Для добавления измений в коммит используется команда *git add*. Чтобы использовать команду *git add* напишите *git add <имя файла>*

### Просмотр состояния репозитория
Для того, чтобы посмотреть состояние репозитория используется команда *git status*. Для этого необходимо в папке с репозиторием написать *git status*, и Вы увидите были ли измения в файлах, или их не было.

### Создание коммитов
Для того, чтобы создать коммит(сохранение) необходимо выполнить команду *git commit*. Выполняется она так: *git commit -m "<сообщение к коммиту>*. Все файлы для коммита должны быть ***ДОБАВЛЕНЫ*** и сообщение к коммиту писать ***ОБЯЗАТЕЛЬНО***.

## Перемещение между сохранениями
Для того, чтобы перемещаться между коммитами, используется команда *git checkout*. Используется она в папке с пепозиторием следующим образом: *git checkout <номер коммита>*

## Журнал изменений
Для того, чтобы посмтреть все сделанные изменения в репозитории, используется команда *git log*. Для этого достаточно выполнить команду *git log* в папке с репозиторием

## Работа с удалёнными репозиториями
Для того, чтобы внести вклад в какой-либо Git-проект, вам необходимо уметь работать с удалёнными репозиториями. Удалённые репозитории представляют собой версии вашего проекта, сохранённые в интернете или ещё где-то в сети. У вас может быть несколько удалённых репозиториев, каждый из которых может быть доступен для чтения или для чтения-записи. Взаимодействие с другими пользователями предполагает управление удалёнными репозиториями, а также отправку и получение данных из них.

### Добавление удалённых репозиториев
Для того, чтобы добавить удалённый репозиторий и присвоить ему имя (shortname), просто выполните команду git remote add <shortname> <url>:

### Получение данных из удалённых репозиториев
Для получения данных из удалённых проектов, следует выполнить: git fetch [remote-name]

### Отпрвка данных в удалённый репозиторий
Когда вы хотите поделиться своими наработками, вам необходимо отправить их в удалённый репозиторий. Команда для этого действия простая: git push <remote-name> <branch-name>. Чтобы отправить вашу ветку master на сервер origin (повторимся, что клонирование обычно настраивает оба этих имени автоматически), вы можете выполнить следующую команду для отправки ваших коммитов: git push origin master

## Ветки в Git

### Создание ветки

Для того, чтобы создать ветку, используется команда *git branch*. Делается это следующим образом в папке с репозиторием: *git branch <название новой ветки>*

## Слияние веток

Для того чтобы дабавить ветку в текущую ветку используется команда *git merge <name branch>*

## ~~Удаление веток~~
Для удаления ветки нужно ввести команду "git branch -d 'name branch'", где вместо "name branch" нужно будет написать имя нужной ветки.

## Основные команды Git
* git init - инициализация локального репозитория
* git status - получить информацию о текущем состоянии git
* git add - добавить файл(файлы) к следующему коммиту
* git checkout - переход от одного коммита к другому
* git log - вывод всех коммитов и и хешей
* git log - вывод на экран всех коммитов
* git diff - увидеть разницу между текущим файлом и закоммиченным файломпше

Это [официальный сайт](https://git-scm.com) git, на котором можно прочитать документацию и скачать git

### Логотип Git
![logoGit](https://fuzeservers.ru/wp-content/uploads/3/d/0/3d04c77fc4b28183e47e091b125bf1a1.png)

#### Вот что говорит о git его создатель Линус Торвальдс:
>Я очень доволен Git. Он работает исключительно хорошо с кодом ядра и по-прежнему следует моим ожиданиям. Что интересно, так это то, что он принял так много других проектов. К удивлению быстро, в конце концов. Существует много инертности в переключении от одних СКВ к другим; только взгляните как долго оставались в использовании CVS и даже RCS, но на каком-то этапе Git принял и их дела.