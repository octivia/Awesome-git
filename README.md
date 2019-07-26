# Awesome-git
/*
  
  1. This text file will be guide for the git and the github 
  2. We will be learnig git and learn how to handle the github

*/

//1. To deploy the project in the github 
//Steps
1. Make New repository in the github 
2. Open the git bash
3. navigate to the project which you want to deploy
4. git init --> this will initialize the repository in local directory
5. git remote add origin "link of the github  repository"  --> this will make the remote repo as a origin 
6. git status ---> to check the status of the files (untracked ,modified)
7. git add file_name --> to add the files into the stace so that we can commit the file later on 
8. git commit -m "write any message for your first commit"
9. git add -A --> to add the all the files into the one place 
10. git commit -a  -m "message for the commit changes " --> to commit all the files in one go
11. git log --> to track the all the process of the git 

/*
 Types of the branches 
1. Local branches --> which are locally 
2. Remote-tracking branches ---> which can be access remotly

*/

12. git branch branch_name --> to create the new branch 
13. git checkout branch_name ---> to move the new branch 

/*

  Merging of the branches when we are done with any extra features or the extra
  functionality  in the project  
  **1. First go the master branch  using git checkout 
*/

14. git merge branch_name  --> it will merge the branch and the master branch

//But if we are in branch and we commit the new changes 
//then it won't affect the master branch. 
//To see the changes we need to merge the again 
 


/*
  
  Parallel Development - Rebasing 
  1. This is alos a way of combining the work between different branches 
  2. It can be used to make a linear seqences of commits

*/
1. Go to the another branch 
2. git rebase master ---> It will make the new branch up to date
3. Go to the master branch 
4. git rebase branch_name ---> It will merge all the files in the master file 


/*

 Generating ssh-key  to secure the repository 
  

*/
1. ssh-keygen --> will generate the ssh key 
2. Add the ssh in github --> Go to setting --> SSH and GPH
3. ssh -T git@github.com --> To authenticate the ssh key 

/*
Revert back : It is the process to go back to previous version 
*/
1.  Create new file and add that file in to the master branch 
2.  commit the newly created file into the master branch 
3.  modify the file 
4.  commit the file to see the changes in the newly created file 
5.  Now revert the file 
6.  Check the log of the git using git log 
7.  Now the first 8 hash of commit 
8.  Run the command 
9.  git checkout copied_hash_value  file_name  --> this will revert back to previous version
