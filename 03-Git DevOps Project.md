we will perform the below task as a devops engineer.

1. Create a private repository
2. Create 3 branches (Dev, UAT and Prod)
3. Add team as collaborators to this repo
4. Enable SSH based authentication
5. Protect Prod and UAT branches
6. 1 approval is needed to check in the code in UAT and 2 approvals needed to check in the code in Prod
7. Build and Deploy should be successful before check-in the code to UAT and Prod branch

**LAB
create a repo in github
mark it as private
add readme file and create
go to code > branches
create 3 branches with name dev, uat and prod
go to all branches and make dev as default branch
then delete master branch

** Protecting uat and prod branches
go to settings > branches
add branch protection rule // can be done only paid version
add branch name and add reviewers

** Add collaborators
go to settings
manage access
invite collaborators

** Enable ssh authentication
https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent
run ssh keygen command in all developer system
adding ssh keys to agent
start the ssh agent in the background
eval $(ssh-agent  -s) //run the command in all the developer machine

add ssh private keys to  ssh-agent
ssh -add ~/.ssh/id_rsa

go to github account
settings >> keys >> SSH and GPG keys
click on New SSH keys

titile - developer machne name
key - for the key go to developer machine command prompt and run the below command
cat ~/.ssh/id_rsa.pub

Once key is added in github account, developr can clone the repo to their local machine using github ssh url without credentails.
