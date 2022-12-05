# Инструкция для работы с Git и удалёнными репозиториями

## Что такое Git?
Git - это одна из реализаций распределённых систем контроля версий, имеющая как и локальные, так и удалённые репозитории. Является самой популярной реализацией систем контроля версий в мире.

## Подготовка репозитория
Для создание репозитория необходимо выполнить команду git init  в папке с репозиторием и у Вас создаться репозиторий (появится скрытая папка .git)

## Создание коммитов

### Git add
Для добавления измений в коммит используется команда git add. Чтобы использовать команду git add напишите git add <имя файла>

### Просмотр состояния репозитория
Для того, чтобы посмотреть состояние репозитория используется команда git status. Для этого необходимо в папке с репозиторием написать git status, и Вы увидите были ли измения в файлах, или их не было.

### Создание коммитов
Для того, чтобы создать коммит(сохранение) необходимо выполнить команду git commit. Выполняется она так: git commit -m "<сообщение к коммиту>. Все файлы для коммита должны быть *ДОБАВЛЕНЫ* и сообщение к коммиту писать *ОБЯЗАТЕЛЬНО*.

## Перемещение между сохранениями
Для того, чтобы перемещаться между коммитами, используется команда git checkout. Используется она в папке с пепозиторием следующим образом: git checkout <номер коммита>

## Увидеть разницу между файлами
Для того, чтобы увидеть разницу между текущим файлом и закоммиченным файлом используется команда  git diff. 

### Выводить список всех сохранение (коммитов)
Для вывода списка всех сохранений используется команда git log

### Переход на актуальную сохраненную версию
Для перехода на самую актуальную версию используют команду git checkout master

## Ветки в Git

### Создание ветки

Для того, чтобы создать ветку, используется команда *git branch*. Делается это следующим образом в папке с репозиторием: *git branch <название новой ветки>*

## Слияние веток

Для того чтобы дабавить ветку в текущую ветку используется команда *git merge <name branch>*

## Удаление веток
Для удаления ветки ввести команду "git branch -d 'name branch'"

## Журнал изменений
Для того, чтобы посмтреть все сделанные изменения в репозитории, используется команда *git log*. Для этого достаточно выполнить команду *git log* в папке с репозиторием. 

Git log --graph -увидеть все ветки с сохранениями. 

## Удаленный репозиторий

Для создания удаленного репозитория создается аккаунт на Github.com, далее в нем создается локальный репозиторий. Затем необходимо "подружить" локальный и удаленный репозитарий. Далее необходимо отправить локальный депозитарий путем ввода кода git push в Терминале в удаленнный депозитарий. 