# Commits
git log //to see the commit history
HEAD will always points to latest commit, meaning the latest updated content of the repository
git diff <commit id1> <commit id2> //you can take the complete commit id or the first 4 to 7 characters of the commit id
  red highlighted color with - symbol means those lines are added to the latest file
  green highlighted color with + sign means those lines are deleted
  white color means no changes made to those lines

* git diff HEAD HEAD~1 //HEAD is latest commit and HEAD-1 is immidiate previous commit. this is not minus symbol, but tilde symbol
similarly HEAD~2 is 2nd previous commit and so on.

**Show the changes made to a specific commit**
git show <commit id>

**How many people worked on a specific file**
git annotate <filename>

commit id is nothing but a SHA code (Secure Hash Algorithm)

In github, we can see these in a graphical way without any command.

# Brancheing Strategy
### Devops high level workflow
**SCM > Build > Unit Testing > Code Quality Analysis > Code Security Analysis > Artifact Repository > Deployment Tool > Hosting Server**

git branch //list all the branches available
git branch test //create a branch with name test
git switch - //switch to prev branch

git checkout -b dev //it will create a branch called dev and also switch to dev branch

To check what is the current branch
git log // HEAD is pointing to current branch

git checkout <branch name>

**Merging**
git checkout <destination branch name>
git merge <source branch name>
git push origin <destination branch>

**Merge conflicts**
Whenever more than one developer change the same file and same line of code, then merge conflict will happen.
In this case, both developer sit togethere and manually edit the file and decide which line of code should be comitted.

### Forking a Repository
git clone will clone the repo from remote i.e. from github account to local machine
forking is used to clone repo from one github account to another github account.

login to your target account. Search the repo in search bar which you want to clone and click on fork. 
![image](https://github.com/user-attachments/assets/4b055416-6971-4f76-b0ae-2098f31fb84e)

Creating pull request
others github account >Fork the repo> to developer github account >clone the repo> to local machine
do changes > commit to local repo > push changes to developer github account >> push to others github account




### Reference for branching
https://git-scm.com/book/en/v2/Git-Branching-Branches-in-a-Nutshell


