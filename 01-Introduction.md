**What is version control**
  A system keeps records of your changes
  Allows for collaborative development
  Allows you to know who made what changes and when
  Allows you to revert any changes

**Types of version control**
  Local - applicable for single developer
  Centralized - Collaborative development. It has main server repo and developers can connect to server for any changes. Does not have local copy in developers machine as local repo.
  Distributed - It has main server repo and also local repo in developers machine. developer can sync to server for latest changes.

git environment lab
  developer-1 - windows user - install git on windows
  developer-2 - linux user - install git on linux on a cloud vm

  after installing check - git --version

Intoduce yourself to git [This is one time activity after installing git]
git config --global user.name "sandeep"
git config --global user.email "tripathy.sandeepkumar@outlook.com"

**To display details**
git config --global user.name
git config --global guser.email

**Initializing a working directory**
create a folder in c drive
go to git bash command promptv - either right click inside folder and select git bash or from command prompt, go to that folder
  git init .
create some sample files


**Git Stages**
Working directory >> (git add) >> Staging or Index area >> (git commit) >> Repository [Local Repo] >> git push >> Remote Repo
Remote Repo >> git clone/pull >> working directory

git status
git file1 file2 file3
git add .
git add -all

all the above 3 commands will add the files to staging area.

git log //will show the commit history
git commit -m "add to repo"v //added to local repository

compare the working directory files (highlighted in red color) and staging area files (highlighted in green color)
git diff
compare the staging directory files and local repo files
git diff --staged

git diff --staged HEAD //compare changes of working directory with local repo

git clone <repo url> //it will copy the remote repo to our working directory
after you work on the changes, push the code to remote repo
git status
git add .
git commit -m "added files"
git push origin master

**git clone vs git pull**
git clone is used when the repo does not exist in our local system.
if repo is there and we need to copy the files only, then git pull command is used.


**Summary**
create a working directory or work space in your local drive
create the project with necessary files
go to git bash command prompt, navigate to workspace directory and initialize the directory
git init .
git status
git add .
git commit -m "1st commit"
Now we have to push these to remote repo
login to github and create a repository
create repo without adding readme file or any default files
git remote add origin git@github.com:orgname/reponame.git
cat .git/config //you can see the remote origin added in the config file
git branch --set-upstream-to=origin/master master
git push origin master


