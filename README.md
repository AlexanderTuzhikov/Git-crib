# Шпаргалка по Git и GitHub

## Инициализация проекта

```bash

git init Инициализировать репозиторий в текущей папке
```

## Статус и история

```bash

git status Показать текущие изменения
git log История коммитов
```

## Добавление файлов

```bash

git add filename Добавить файл в индекс
git add . Добавить все изменения
```

## Коммит изменений

```bash

git commit -m "Сообщение" Зафиксировать изменения
```

## Подключение к удалённому репозиторию

```bash

git remote add origin git@github.com:USER/REPO.git
git remote -v Проверить удалённый адрес
```

## Отправка на GitHub

```bash

git push -u origin master Первый пуш (если ветка master)
git push Следующие пуши
```

## Клонирование репозитория

```bash

git clone git@github.com:USER/REPO.git
```
## Получение изменений

```bash

git pull Стянуть последние изменения
```

## Работа с ветками

```bash

git branch Показать все ветки
git checkout -b new-branch Создать и переключиться на ветку
git checkout main Переключиться обратно
git merge branch-name Влить ветку в текущую
```

## Удаление

```bash

git branch -d branch-name Удалить локальную ветку
git remote remove origin Удалить подключение к удалённому репо
rm -rf .git Удалить Git из папки
```

## Настройка SSH (один раз)

```bash

ssh-keygen -t ed25519 -C "email@example.com"
ssh-add ~/.ssh/id_ed25519
cat ~/.ssh/id_ed25519.pub Копировать в GitHub → Settings → SSH Keys
```

## Полезное

```bash

git config --global user.name "Имя"
git config --global user.email "email@example.com"
```