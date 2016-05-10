Git Cheatsheet
==============

Create a new repo in a local folder : git init
----------------------------------------------

git init


Get a remote repo, e.g., from github : git clone
------------------------------------------------

git clone <remote url>


Link a remote repo to a local repo : git remote add
---------------------------------------------------



Update staging area : git add
-----------------------------

add one or more files: git add <filename1> <filename2> <...>

add all files in local directory: git add .

add all files recursively: git add -A


Commit files : git commit
-------------------------


Get status : git status
-----------------------


Get history : git log
---------------------


Create a new branch : git branch
--------------------------------

git branch <newBranchName>


View list of branches : git branch
----------------------------------

git branch


Switch to a different branch : git checkout
-------------------------------------------

git checkout <branchName>


Get a file from the staging area : git checkout
-----------------------------------------------

git checkout <fileName>


Delete a branch : git branch
----------------------------

git branch -d <branchName>


Merge changes into the current branch : git merge
-------------------------------------------------


Get remote data (into .git folder, leave working directory unchanged) : git fetch
----------------------------------------------------------------------------------


Get remote data (into .git folder, update working directory to current remote status) : git pull
------------------------------------------------------------------------------------------------


Update remote with local commit : git push
------------------------------------------
