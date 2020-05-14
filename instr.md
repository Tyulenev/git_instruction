Инструкция по работе  GIT
git init - инициализация локального репозитория

git status - ПРоверить статус репозитория

git log - вывод логов (gfhfvtnh -oneline)
git reflog - полный логов (все события* переход по истории и т.д.)
git reset "hasgcommit" - сбрасывает состояние по хэшу 
git revert - отмена конкретного commit'a
git restore - Сброс конкретногг файла

git branch
git branch dev
git chekout -d ВЕТКА - Удалить ветку
git chekout -b ВЕТКА - Перейти и добавить ветку


git push
git pull
git fetch

git add . - добавление всех фалов в @antracked

//Генерирование ssh key
ssh-keygen


git merge
git rebase
git push --force

git tag 1.0.0 - добавляет версию к текущему коммиту
git push --tags - добавляет тэг в удал. репозиторий
git tag -d 1.0.1 - Удаляет тэк в локально репозитории
fit push --delete origin 1.0.1 - удаляет тэг в удаленно репозитории