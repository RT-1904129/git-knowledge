# git-knowledge
Discription of git\
1)git(Distributed Version Control System)  means Everyone has a copy of the entire repositry with the entire version history .
- A software used to tracking changes in set of files .
- A git Repository(Repo) is like a database which maintains different version of Project files.
- These Versions or Snapshot are refered as Commit in Git Terminology.
**Modefied Files** These are the files which are modified after the latest snapshot .
**Staged Files** The set of files which are about to be committed to create a new snapshot .
**Committed Files** These are the Unmodified files which are same since the latest commit .
 - **Git creates a snapshot of all the changes that are part of staging area.**
Configure who get credit for the changes made from your device by setting the author details from your terminals
- git config --global user.name "Your Name" 
- git config --global user.email "youremailaddress@example.com" \
to set automatic command line coloring for Git for easy reviewing 
- git config -- global color.ui auto
There are several cloud-based repository hosting services which let you maintain a copy of repositry
- Github
- Bitbucket \
2) we can do Trunk based devlopment. In mac it already install but for windows we need to downlode git base.\
3) github,gitlab,Bitbucket are git profarmer options. \
###############  Git commands on git base ################\
1) for making clone(making same copy of it) of any github reprository use---\
git clone (repo path but donot put braket like this)\
2) for adding changes on github repro which you made on clone copy simentenously use three commandas one after one----\
3) Firstly we need to added the changes in staging area by this command we are adding changes in staging area. \
i)git add path\
ii)git commit -m "commit message"
- after that we need to push the things in remote repositry from our local repositry \
iii)git push -u origin (branch name in which you want to do change but donot put bracket like this there mostly main or master)\
3) If any other contributer contribute in your repository and you want to put that changes in your clone copy just use this command-----\
git pull origin (branch name in which changes happen don't put bracket like this main or master)\
4) If you want to know that in which branch you are present know use this command---\
git branch \

5) If you want to create a new branch(but your are present stay at old branch you are not directly went to new created branch) but this craeted brach is locally created in your system you need to make it globally) \
git branch (new branch name don't put bracket like this)\
than type command --- \
git checkout (branch name) \
git push -u origin branchname

6) If you want to move from current branch to another branch than use this command as-----\
git checkout (branch name but don't put the bracket like this)\
7) If you want to creat a new branch and you want simentenously move to that newly created particular branch than use this command-----\
git checkout -b (new branch name but don,t put bracket like this there)\
for making it global(remote server) we will type command as \ 
git push -u origin branchname 

8) If you want to check status of current status  git kernal than use this command---- \
git status
9) to know from which website we clone the things in git repositry type command as------\ 
git remote -v
10) To inisilize any folder as git repositry file go inside folder type command as ----\
git init
11) we can be configure a remote repositry to local **repositry** (that file should be in git formate eans initalize with git )  by command as \
git remote add origin URL
12) Command to list all commits --\
 git log 
 
Output:- 
commit d8d879259ccd24fe7f8bbaa5ee499321bc7377b4 (HEAD -> master)
Author: Rishabh Tripathi <rishabh29072001@gmail.com>
Date:   Sun May 29 18:44:02 2022 +0530

    tesing github
- Commit IDs are  unique string(hashes) that are created whenever a new commit is recorded 
13) to know unstagged changes commnd \ 
git diff 

14) to show that staged and uncommitted changes we use command as \ 
git diff --staged

15) suppose you want to store your work in back and donot count in commit and when you want to get it you can get this so type command \
git add . \
git stash \
** Now if you want to back this work type command** \
git stash pop \
** but if you type -- git stash clear -- than you will never get that ** \
16) To delete any branch type command --- \
git branch -D <branch name> 
17) git fetch + git merger == git pull
 
 18) how to merge brach in main
 git merge (branch name)
 
 19) Rebasing do much clean  branch history adding all brach in one branch \
 git rebase (actual branch)
 
 20) how to uptodate our main repositry from remote repositry of any forked project (firstly go in main branch) \
 git rest --hard upastream/main \
 git push origin main \
 
 - And we can do it by **git pull upstream main**
 
21) how to see all your previous commit History \
 git reflog \
22)Undoing Committed Changes (Git Reset)
 git reset --hard commitID \
 Link ->https://www.cloudbees.com/blog/git-undo-commit
 
23) git command to add remote repositry \
 git remote add origin git-repositry-url
24) git command to add changes in previous commit is  \
  git commit --amend
