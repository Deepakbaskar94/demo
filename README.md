# GIT Commands
demo to teach git


# Heading
this is readme file

Git and Github

********************************************************************************************
1. to download the complete code of the repository

git clone url

********************************************************************************************
2. to open it in the VS code (get inside the base folder which we downloaded)

code .

********************************************************************************************
3. to add the edited program to the github repository

git add .\add.py

********************************************************************************************
4. to see the files need to be committed

git status

********************************************************************************************
5. it happens in local computer (kind of creating a check point)

git commit -m "message for reference"  #to add the files whichever is added in the previous comand
git commit -am "message for reference" #to commit all changes at once

********************************************************************************************
6. to push the code to the github website

git push

********************************************************************************************
7. to get updated in the local system (if someone changed after we downloaded to update)

git pull

********************************************************************************************
8.merge conflict during git pull

<<<<<<<< HEAD (Current Change)
a = 15   	#what we did in local repository
======
a = 22		#what somebody did and updated in the github
>>>>>>>> 7c6bdsgisjoglgjakiueo (Incoming Change)
b = 2
print (a + b) 

#change to

a = 15
b = 2
print (a + b) 

git commit -am "corrected the merge conflict"
git push #to push it to github


********************************************************************************************
9. reset to previous commit or to origin commit

git reset --hard<commit hash>
git reset --hard origin/master

********************************************************************************************
10. git branching concept

to know which branch we are in
git branch  

to create a new brach and switch to that branch
git checkout -b "new_branch_name"
git branch

to switch to another branch
git checkout existing_branchname

to merge the two branches 
check the current branch name
check which branch need to be merged
if we are in master and if we want to merge the newbranch

git merge newbranchname

 *****************************************************************************************
11. remote origin
  
  to know remote origin 
  git remote
  
  to know remote origin url
  git remote -v
  
  to remove the remote origin
  git remote remove origin
  
***************************************************************************************** 
  
12.  For VS code configuration and push from device
  
git config -l --show-origin

git config --global user.email "deepakbaskar@outlook.com"
git config --global user.name "deepakbaskar94"

git remote add frappe-test https://github.com/Deepakbaskar94/frappe-test

git add .
git commit -a -m "first commit of frappe"
git push frappe-test   //frappe-test is repository name
git push --set-upstream frappe-test master
  
  
