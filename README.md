# Delete-file-.idea


# Удаление файла .idea 

Очень часто при создании проектов в PhpStorm от компании JetBrains при первом коммите народ по привычке нажимает «ОК» на все вопросы IDE и папка .idea попадает в git-репозиторий, которой там совсем не место. Удаляется оттуда она очень просто.
____

```
# Добавить папку в игнор-лист гита
echo '.idea' >> .gitignore
 
# Удалить папку из стейджинга
git rm -r --cached .idea
 
# Добавить файл в гит
git add .gitignore
 
# Зафиксировать изменения
git commit -m 'Удалил папку .idea из репозитория'
 
# Запушить в репу
git push
```

Сами ребята из JetBrains [рекомендуют](https://github.com/github/gitignore/blob/master/Global/JetBrains.gitignore) .gitignore
