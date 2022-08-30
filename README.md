# Инструкция для работы с Git и удалёнными репозиториями

## 1. Что такое Git?
**Git** - это одна из реализаций распределённых систем контроля версий, имеющая как локальные, так и удалённые репозитории. Является самой популярной реализацией систем контроля версий в мире.
## 2. Подготовка репозитория
Для создания репозитория необходимо выполнить команду _**git init**_  в папке с репозиторием, и у Вас создаться репозиторий (появится скрытая папка **.git**).

## 3. Создание коммитов

* ### Git add
Для добавления измений в коммит используется команда _**git add**_. Чтобы использовать команду _**git add**_ напишите _**git add <имя файла>**_.

* ### Просмотр состояния репозитория
Для того, чтобы посмотреть состояние репозитория используется команда _**git status**_. Для этого необходимо в папке с репозиторием написать _**git status**_, и Вы увидите были ли измения в файлах, или их не было.

* ### Создание коммитов
Для того, чтобы создать коммит(сохранение) необходимо выполнить команду _**git commit**._ Выполняется она так: _**git commit -m "<сообщение к коммиту>"**_. Все файлы для коммита должны быть ***ДОБАВЛЕНЫ*** и сообщение к коммиту писать ***ОБЯЗАТЕЛЬНО***.

##  4. Перемещение между сохранениями
Для того, чтобы перемещаться между коммитами, используется команда _**git checkout**_. Используется она в папке с репозиторием следующим образом: _**git checkout <номер коммита>**_.

##  5. Журнал изменений
Для того, чтобы посмтреть все сделанные изменения в репозитории, используется команда _**git log**_. Для этого достаточно выполнить команду _**git log**_ в папке с репозиторием.


## 6. Работа с изображениями

Чтобы вставить изображение в текст, достаточно написать следующее
![такси в Индии!](2111062331257203_2834.jpg)

## 7. Синтаксис языка Markdown

* ### Выделение текста

Чтобы выделить текс курсивом, необходимо обрамить его звездочками (*) или знаком нижнего подчеркивания (_). Например, *вот так* или _вот так_.

Чтобы выделить текст полужирным, необходимо обрамить его двойными звездочками (**) или двойным знаком нижнего подчеркивания (__).Например, **вот так** или __вот так__.

Альтернативные способы выделения текста жирным или курсивом нужны для того, чтобы мы могли совмещать оба эти способа. Например, _текст может быть выделен курсивом и при этом быть **полужирным**_.

* ### Списки

Чтобы добавить ненумерованные списки, необходимо пункты выделить звездочкой (*) или знаком +. Например, вот так:

* ##### Элемент 1
* ##### Элемент 2
* ##### Элемент 3
+ ##### Элемент 4

Чтобы добавить нумерованные списки, необходимо пункты просто пронумеровать. Например, вот так:
1. ##### Первый пункт
2. ##### Второй пункт

Чтобы выделить ненумерованный список, используйте (*)

## 8. Ветки в Git


* ### Создание ветки

Для того, чтобы создать ветку, используется команда _**git branch**_. Делается это следующим образом в папке с репозиторием: _**git branch <название новой ветки>**_.

* ### Слияние веток

Для того чтобы дабавить ветку в текущую ветку используется команда _**git merge <name branch>**_.

* ### Удаление веток
Для удаления ветки ввести команду **"git branch -d 'name branch'"**.

## 9. Работа с удаленными репозиториями

* ### __git clone <http:... >__
Команда позволяет склонировать внешний репозиторий на наш ПК. Команда **git clone** составная: она не только
загружает все изменения, но и пытается слить
все ветки на локальном компьютере и в
удаленном репозитории.

* ### __git pull__
Эта команда позволяет скачать все из текущего репозитория и автоматически сделать merge с нашей версией. 

* ### __git push__
эта команда позволяет отправить нашу версию репозитория на внешний
репозиторий. **ТРЕБУЕТ АВТОРИЗАЦИИ** на внешнем репозитории.

* ### __Как сделать pull request__

 --- Делаем *fork* репозитория

 --- Делаем clone СВОЕЙ версии репозитория

 --- Создаем новую ветку и в НЕЕ вносим свои изменения

 --- Фиксируем изменения (делаем коммиты)

 --- Отправляем свою версию в свой GitHub

 --- На сайте GitHub нажимаем кнопку *pull request*
