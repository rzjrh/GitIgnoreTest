# GitIgnoreTest

//gitignore 
//1- create new directory add all the project files in the directory 

//2- open git bash 
 
cd (project directory)
git init

touch .gitignore
touch test1.txt test2.txt test3.txt test4.txt
touch test.html
touch style.css
touch secret.js

vim .gitignore

//3- now edit the gitognore file 
	*.txt
	secret.js
	
//close the vim (ESC :q!)

git status  //make sure the .txt files and secret.js are not listed 

git add .
git commit -m "first commit with .gitignore"
git status

git remote add origin https://github.com/rzjrh/GitIgnoreTest.git
git push origin master 
git clone https://github.com/rzjrh/GitIgnoreTest.git

//you will see only test.html uploaded in the github


