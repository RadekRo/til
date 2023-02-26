# git 
### basic commands

Cloning **remote** repository to current catalogue (creates subcatalogue with repository name!)
```git clone <repository url address>```\
Getting all current changes made to **remote** repository
```git pull origin <branch>```\

Show current **local** repository/branch status
```git status```\
Show all logs of **local** repository/branch
```git log```\
Show all current **local** repository branches (**notice** that your current branch will begin with __*__ mark.)
```git branch```\
Create new **local** branch
```git branch <new branch name>```\
Switch on **local** branch
```git checkout <branch>```\
Merge current **local** branch (on witch you are currently set) with given *branch*
```git merge <branch>```\

Include *file* change in the next commit
```git add <file>```\
Include *all changes* in the next commit
```git add .```\
Commit **all** the added changes.
```git commit -m "your comment goes here"```\

Send commited changes to your **remote** repository branch (**notice** that if you leave the branch empty - all branches will be sent)
```git push origin <branch>```\

---
_Last update: 23 Feb 2023_ 