# Ресурсы
[Работа с коммитами](https://igorsmolin.ru/2020/03/23/%D0%B1%D0%B0%D0%B7%D0%BE%D0%B2%D0%B0%D1%8F-%D1%80%D0%B0%D0%B1%D0%BE%D1%82%D0%B0-%D1%81-%D0%BA%D0%BE%D0%BC%D0%BC%D0%B8%D1%82%D0%B0%D0%BC%D0%B8-%D0%B2-git/)
[Хабр: 10 Git-комманд, которые стоит знать разработчику](https://habr.com/ru/company/skillbox/blog/442260/)
[Хабр: Git на практике](https://habr.com/ru/post/342116/)

[Ветвление с примерами из реальной жизни](https://proglib.io/p/vetvlenie-git-s-primerami-iz-realnoy-zhizni-2020-01-25)

[Bitbucket: Конфликты слияния в Git](https://www.atlassian.com/ru/git/tutorials/using-branches/merge-conflicts)


# Команды

## Инициилизация репозитория git

```console
git init - инициализация репозитория
git clone <URL коммита> - клоннировать репозиторий
```

## Работа с commit-ами

```console
git status - вывести справку о текущем состоянии репозитория
git log - посмотреть историю коммитов
git log --pretty=format:"%H [%cd]: %an - %s" --graph --date=format:%c
```

```console
git restore <имя файла> - отменить изменения
git restore . - отменить все изменения

git add <имя файла> - добавить файл в репозиторий
git add . - добавить все файлы в репозиторий
git commit - закоммитить изменения
```
```console
Как выйти из редактора Vim?
    1. Нажимаем i.
    2. Вводим заголовок коммита в первой строке.
    3. Пропускаем строку (Enter) и вводим текст тела коммита (желательно)
    4. Нажимаем Esc.
    5. Вводим :x.
    Вы свободны!
```

```console
git commit -m '<cообщение коммита>' - закомитить изменения, и ввести сообщение коммита без перехода в редактор
git commit --amend - добавление поэтапных изменений в последний коммит
git reset HEAD~ - отменить последний коммит в локальном Git репозитории
git reset --hard HEAD~1 - полностью удалить последний коммит
git checkout <hash коммита> - переключить рабочую дирректорий на состояние предыдущего коммита
git revert <hash коммита> - отмена изменений в коммите.
```
## Работа с ветками

```console
git branch
git branch --list - посмотреть список локальных веток
git branch –r - посмотреть список удаленных веток
git checkout –b <имя новой ветки> - создать новую ветку из текущей и переключиться на нее
git branch <имя ветки> - создать новую ветку из текущей без переключения
git checkout <имя ветки> - переключиться на существующую ветку
git branch -m <новое имя ветки> - переименовать существующую ветку
git merge <имя ветки> - влить изменения из другой ветки в текущую
```
## Обновление репозитория и отправка изменений

```console
git fetch –all - извлечение всех последних изменений из удаленного репозитория
git pull
git push <Remote.> <Branch.> - отправка изменений на удаленный сервер
```



## Разрешение конфликтов

```console
cat <имя файла> - открыть файл в текстовом редакторе коммандной строки
git log --merge - вывести список файлов, конфликтующих во время слияния
git merge --abort - отмена слияние и возвращение к предыдущему состоянию
```

### Прочее

```console
git reflog —  показать журнал изменений в заголовке локального репозитория. Отличный вариант для поиска утраченных данных.

git clean — удаление неотслеживаемых файлов в локальной рабочей директории.

    -n — флаг для пробного запуска, ничего не удаляется
    -f — флаг для удаления файлов
    -d — флаг для удаления неотслеживаемых директорий
```