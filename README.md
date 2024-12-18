# Команды для Git
___

git config --list --show-origin

git config --global user.name "имя"

git config --global user.email "youremail@example.com"

git config --list - Проверка настроек

git init

git status - запрашивает текущее состояние репозитория

git add .

git config --global core.editor "code"

git commit -m "Сообщение"

git remote add origin URL  - указывает, что вы добавляете удаленный репозиторий с указанным именем URL в качестве origin локального репозитория Git.

git push --set-upstream origin master - отправить нашу главную ветку на исходный URL-адрес и установить ее в качестве удаленной ветки по умолчанию

git remote remove origin - удалить репозиторий из Git

git push -u origin master - добавить проект на github

git remote -v - проверить подключён ли репозиторий в Git

git commit --amend -m "Сообщение"

.gitignore

https://cbea.ms/git-commit/#separate

*.txt      //* - любая последовательность символов   a.txt ab   1234.txt

//a1a.log  a1234a.log   a2a.log

a?a.log  //? - один символ, а не группу символов

//b1b.log b2b.log b3b.log

b[12]b.log
b[6-9]b.log
b[1][0]b.log //b20b.txt b??b.txt
b[1]?b.log //b11.log b12.log ...
//c1c.log c2c.log c3c.log
c[!2]c.log

test/*

git show 28400179194c53b75972d3c3a86f83bd08669156

52272f84a675979ff843e320d91715b7fb6ed1ba

git log --grep="1.34.31"

git log --stat

git log -p  //git log --patch

git log --oneline

git tag
git tag -a v1.0
git tag -a v1.0 -m "Message"

git branch

git branch "название"

git branch -f main HEAD~3

git checkout <название>

git branch -d "название"

git merge <название>

git checkout -b "name"

https://learngitbranching.js.org/?locale=ru_RU

a.txt  b.txt  c.txt  d.txt e.txt        
                     1.txt 2.txt 3.txt

1.txt 2.txt 3.txt 4.txt 5.txt

git reflog

git commit --amend

git revert <номер коммита>

git reset --hard <номер коммита>

New-Item -ItemType File -Path ".\README.md"

# Команды для Github CLI
___

sudo apt install gh - установка github cli

gh auth login - вход в github cli

gh auth status - проверка вошли ли вы в систему и активна ли аутентификация для выполнения действий на GitHub

gh --version

gh auth logout

gh repo create "имя репозитория" --public - создание удаленного репозитория на Github
