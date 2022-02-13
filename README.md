# Git-and-github-notes

- mkdir, to make a folder 
- mkdir project 
- ls
- cd project 
- git init - to initialise empty git repository 
- ls-a ( to see what is hidden in the folder)
- ls.git 
- touch names.txt ( This is done to make a new file)
- git status 
- git add. ( everything that is there in the folder that has not been added gets added)
- git add names.txt ( add only the particular file) 
- git status ( as now you have added names.txt, this folder would be in green ) 
- git commit -m "Names.text files added" ( m is the message that needs to be added) 
- git status 
- cat names.txt ( It displays whatever things are visible in the names.txt file) 
- git status 
- git add . 
- git status 
- git restore --staged names.txt 
- git status - They are outstide the stage 
- git add names.txt 
- git commit -m "Names.txt file modified"
- git log  ( The history of the project) 
- rm-rf names.txt (To delete the file) 
- git status 
- git add. 
- git commit -m "The names.txt file was deleted"
- git log 
- If these were done by mistake, we can unstage each commits 
- To remove the commits above, just copy the latest commit 
- Git reset and paste the latest copied commit 
- git log 
- git stash 
- git status 
- git log 
- git stash pop 
- git add . 
- git stash 
- git stash clear 


## To push code into the project 

- git remote add origin  ( paste the url of the project here ) 
- git remote -ve ( This shows all the urls that is attached to the original folder) 
- git push origin master 

## What are branches? Merging Braches to main 

- git branch feature 
- git checkout feature  - ( all the new commits that I will be making will be added on the feature branch) 
- git commit 
- git commit 
- git checkout main 
- git commit 
- git merge feature 
- git checkout c5 
- git checkout c8
- git checkout main 
- git log 
- git push origin master - ( to push all the code to the main branch) 

## Why Fork and how to Fork 

- git clone ( and paste the url of that repository ) 

## What is Upstram and adding it to local 

- git remote add upstream ( add the link of the repository) 
- git remote -v 

## What is a Pull request 

- git status 
- git branch Thivyaa
- git checkout Thivyaa ( head is now changed to Thivyaa, all the commits I make will go to this branch) 
- git add . 
- git commit -m "Thivyaa added a message"
- git log ( Never commit on main branch) 
- git push origin Thivyaa 
- ( For every feature, bug you are working on create a new pull request, if a branch alrady has a pull request, it will never allow you to commit) 
- ( 1 pull request means 1 branch, one branch can only open one pull request, if you want to create different prs, for different features you are working on the project, we need to create different branches, so that it does not get mixed up.) 
-  git status 
-  git log 
-  To remove copy the feature , you want get removed and add git reset ( paste the link ) 
-  git status 
-  git add . 
-  git stash 

## Making forked project even with the main project 

- git fetch --all --prune
- git reset --hard upstream/main
- git log 
- git push origin main 
- git pull upstream main 
- git push origin main 

## Squashing Commits, Merge conflicts 

- git branch temp 
- git checkout temp 
- touch 1 
- git add . 
- git commit -m "1"

## Merge Conflicts

- If there are many persons who are suggesting changes in the line number 3, git will get confused, 

