# GitCommands
GIT COMMANDS :-
**********************************************
Create a repo on github(using no readme file ) and copy the ssh link (if private then ssh other wise simple)
Go to the folder ->do gitbash here or cd path
git config --global user.name "kanchan0912"
git config --global user.email "jkanchan2911@gmail.com
touch .gitignore
(open file ->  jo b file ignore krni h uska naam n folder k liye folder/ n and save it )
git init
git add .
git commit -m "Initial commit"
git status (just to check)
git remote add origin pasteRepolink
git push origin master 
If project is private then go to settings of github -> go to ssh and jpg keys->create new ssh key->keyName
go to ggogle serach for it and copy the command 
ssh-keygen -t rsa -b 4096 -C  "your email"->enter ->enter 
cat copyPathFromTheGivenLines//tail path
Copy ssh key and paste it in sttings of repo
git push origin master
git log to see track and q to quit
*********************************************
GIT ADD
Update
git add .

git add -a //to add all files
git add --a

git add fileName // to add seperate file

***********************************************
UPDATE
agar already files uploaded hai toh git init nhi krna 
git add --a -> commit -> push krna h update krne k liye
**********************************************
DELETE content of repo
rm -rf .git
DELETE A FILE
git rm filename
//deletes a file and stage also 
comit

*********************************************
CLONING
git clone gitLink //name optional h 
********************************************
GIT DIFF// to compare working directory and  staging area 
git diff // to show the difference between2 files
 git diff --staged// to see diff b/w latest and last commit
 *******************************************
SKIP STAGING AREA
git add filnme
git commit -m -a "commit message"
// tracked file ko commit and untracked to nhi krega commit
******************************************
RENAME
git mv first.txt rename.txt
// renaming a file
*********************************************
TO UNTRACK A FILE
git rm --cached filename
TO UNSTAGE
git restore --staged file name
**********************************************
GIT LOG
git log
git log -p -n
git log -2 //  last 2 commit
git log --stat
git log --pretty=short // one line m saare commit dekhna 
git log --pretty= long// commit kisnr kiya wo 
git log --since  2.days// last 2 din commits
 or 2.weeks,2.
git log --pretty=format:"%h  --%an"
//an author name 
//ae for author email

AMMEND COMMIT
git commit --amen
vim editor i se type , wq se quit'
**********************************************
TO UNMODIFY
git checkout --puraniFIleKaName
git checkout -f // for whole changes
// jb galti se commit krdiya ho aur purane commit pr wapas jana h 
**********************************************
GIT REMOTE
git remote add origin link
git remote// to check

add SsHkey 
*********************************************
GIT ALIAS
shortcommands for big
git config --global alias.st status
git config --global alias.unstage "restore --staged --"
//shortcuts
//status ki jgh st use kr skte h
**********************************************
BRANCHING
git branch // to see all branches
git branch -v // to see hash and commit message
git checkout -b develop or branchName
git checkout master // to go inside any 
git branch --merged// already merged branche
git branch --no-merged // not merged branches
git branch -d branchname //to delete branch  is merged
git branch -D branchname // delete if not merged
existing branch
do the changes
git add .
git commit

MERGING
git checkout master
git merge branchname
conflict resolution marker 
<<<<<
---====
>>>>>
long term branch and topic branch
**********************************************
PUSH
git push message  
git push origin branchName
git push origin branchname:newbranchName
