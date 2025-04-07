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
Working directory >> (git add) >> Staging or Index area >> (git commit) >> Repository [Local Repo]

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




