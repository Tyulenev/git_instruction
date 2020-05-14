Инструкция по работе  GIT
(https://github.github.com/training-kit/downloads/ru/github-git-cheat-sheet/)

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

PULL - Request
git push -u origin Ветка - создает PR для активного коммита в указанной ветке

+++++++++++++++++++
Сложные вопросы!
+++++++++++++++++++
git reset --hard - сбросить репозиторий на поледний коммит

Stash - спец. память для хранения изменений, 
которые не целесообразно пока вносить в коммит
Git Stash - выполняет перенос изменений (текущего проекта) во 
временную локальную память
git stash list - выводит все stash'ы
!!!!   clear
git stash push <file> - добавить file в stash
git stash pop - применить изменения из stasha
git stash

Склеивание коммитов (объединение/сквош)
squash
Можно через merge
1) git merge ВЕТКА --squash
2) git rebase -i HEAD~3 (head - текущ состояние, кол-во коммитов)
-i - интерактивный режим, помогает настраивать

Cherry Pick (Перехвать коммитов)
git cherry-pick hash - перенос коммита в текущую ветку
git cherry-pick <branch> - поледний коммит ветки
git cherry-pick .. <branch> все коммиты ветки

git commit --amend - перезапись поледнеге commita 
!!!	:wq - Чтобы выйти

Разрешение конфликтов
git merge dev1 dev2
Потом status и там будет помечен файл, который вызвал конфликт

