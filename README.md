# lab02
Part 1 

git clone ...
git push -u origin master 
nano hello_world.cpp
git add hello_world.cpp
git commit -m “comment”
nano hello_world.cpp
git commit -a -m “comment”
git push -u origin master 

Part2 

git checkout -b patch1
nano hello_world.cpp
git add hello_world.pp
git commit -m “comment”
git push -u origin patch1
hub pull-request
nano hello_world.cpp
git commit -a -m “comment”
git push -u origin patch1
git push -d origin patch1
git pull
git checkout master
git log
git branch -d patch1 

Part 3 

git checkout -b patch2
clang-format -style=Mozilla -i hello_world.cpp
git commit -a -m “comment”
git push -u origin patch2
hub pull-request
git checkout master
nano hello_world.cpp
git commit 
git push -u origin master
git checkout patch2
git rebase master
nano hello_world.cpp
git rebase —continue
git push -f origin patch2
