# git-knowledge
Discription of git\
1)git(Distributed Version Control System) \
2)we can do Trunk based devlopment. In mac it already install but for windows we need to downlode git base.\
3)github,gitlab,Bitbucket are git profarmer options. \
###############  Git commands on git base ################\
1)for making clone(making same copy of it) of any github reprository use\
git clone (repo path but donot put braket like this)\
2) for adding changes on github repro which you made on clone copy simentenously use three commandas one after one\
i)git add .\
ii)git commit -m "commit message"\
iii)git push origin (branch name in which you want to do change but donot put bracket like this there)\
3) If any other contributer contribute in your repository and you want to put that changes in your clone copy just use this command\
git pull origin (branch name in which changes happen don't put bracket like this)\
4)If you want to know that in which branch you are present know use this command\
git branch\
5) If you want to create a new branch(but your are present stay at old branch you are not directly went to new created branch) (but you are able to see those branches on github when you type all command give in -2) after creating new branche because this created branches is local initally you need to make it global by typing -2)  all three commandes than it directly shows all changes in your new created branches itself )use this command\
git branch (new branch name don't put bracket like this)\
6)If you want to move from current branch to another branch than use this command as\
git checkout (branch name but don't put the bracket like this)\
7)If you want to creat a new branch and you want simentenously move to that newly created particular branch than use this command\
git checkout -b(new branch name but don,t put bracket like this there)\
8) If you want to check status of current status  git kernal than use this command \
git status

