# Commits
git log //to see the commit history
HEAD will always points to latest commit, meaning the latest updated content of the repository
git diff <commit id1> <commit id2> //you can take the complete commit id or the first 4 to 7 characters of the commit id
  red highlighted color with - symbol means those lines are added to the latest file
  green highlighted color with + sign means those lines are deleted
  white color means no changes made to those lines

git diff HEAD HEAD~1 //HEAD is latest commit and HEAD-1 is immidiate previous commit. this is not minus symbol, but tilde symbol
similarly HEAD~2 is 2nd previous commit and so on.

**Show the changes made to a specific commit**
git show <commit id>

**How many people worked on a specific file**
git annotate <filename>

commit id is nothing but a SHA code (Secure Hash Algorithm)

In github, we can see these in a graphical way without any command.

# Branches
### Devops high level workflow
**SCM > Build > Unit Testing > Code Quality Analysis > Code Security Analysis > Artifact Repository > Deployment Tool > Hosting Server**


