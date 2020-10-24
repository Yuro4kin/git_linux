# hellogit
lern git

 git clone git@github.com:YuriyGamiy/hellogit.git hellogit
//  clone repository

npm i 
//  запустили зависимости

git checkout -b "branch_1"
//  создали ветку branch_1 для изменений
//  внесли изменеия в файл readme.md

*git status*  //проверка состояния

git add readme.md
git commit -m "new readme"

git checkout main
//  переключились в основную ветку

git remote add origingit git@github.com:YuriyGamiy/hellogit.git
//  выполнять с main

git push origingit branch_2
//  изменения ушли в main/master репозиторий


*******************************************************
git checkout main
//  перешли в основную ветку
git merge branch_2
//  выполнили слияние из ветки branch_2 в основную main
git branch -D "branch_1"
                     _2
//  выполнили удаление ненужных веток
*******************************************************




