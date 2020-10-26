# hellogit
lern git

 git clone git@github.com:YuriyGamiy/hellogit.git hellogit
//  clone repository

npm i 
//  запустили зависимости

//  если работаем на локальном комп., создали ветку branch_1 и отправили на мастер
    или работаем на локальном комп., создали ветку git checkout branch_1, выполнили слияние в  git merge branch_1 в ветку 1, перешли в основную ветку  git checkout main, и отправили на мастер репозиторий  git push origingit branch_1  ветку 1.

git checkout -b "branch_1"
//  создали ветку branch_1 для изменений
//  внесли изменеия в файл readme.md, создали новый файл, добавили картинку...
*git status*  //проверка состояния
git add readme.md
git commit -m "new readme"

git checkout main
//  переключились в основную ветку

git remote add origingit git@github.com:YuriyGamiy/hellogit.git
//  выполнять с main

git push origingit branch_2
//  изменения ушли в main/master репозиторий, выполнять с main/master ветки.

*******************************************************
git checkout main
//  перешли в основную ветку
git merge branch_2
//  выполнили слияние из ветки branch_2 в основную main
git branch -D "branch_1"
                     _2
//  выполнили удаление ненужных веток
*******************************************************

//С локальной копии main/master создаем ветку git checkout -b "branch_4", выполняем слияние веток  git merge branch_2,   git merge branch_3   ,  перешли в основную ветку  git checkout main, выполнили слияние ветки branch_4 с локальной копией git merge branch_4. Изменения ушли в master/main репозиторий git push origingit branch_4.

********************************************************
// Выполнили fork (личный репозиторий git) с master репозитория, создал у себя локальную копию на комп.,  (поработал с файлами .html, .css), создал ветку git checkout -b "branch_1", отправил изменения в свой fork - git push origin branch_1. Изменения в mаster репозитории pull request выполняется с git только мастером репозитория (проверяет что я сделал, если все ок, то мастер вливает мою ветку). Выполняем git pull gena master - взять все изменения в master репозитории и переместить на локальную машину. Затем git push origin master обновляем свой fork личный репозиторий.

cd .
cd ~
cd dev
git clone ....git@   smart
cd smart               (master)
git remote -v
origin = https
git remote add gena .....git@
git remote -v    // origin  , gena
git checkout -b 'branch_1'
//  изменили файл index.html
git status
git add .
git status
git commit -m "add change index.html"
git push origin branch_1  
//  создал ветку, поработал в файлах
git checkout master
//  переключил на основную ветку
git pull gena master
git status 
git restore "build/css/contacts.css"
git status
git push origin master

******************************************************