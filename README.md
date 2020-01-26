# Repository for Reference - Mac, Github and Maven Commands

## Mac Commands

ps -ef - To list the process and status.  
kill -9 <process id> - To kill a particular process.  
tail -f <file name> - To tail the logs.  

## Git Commands

git config --global http.sslVerify "false"

git config --list - To list all the configuration values.  
git config --list --global - To list all the global configuration values.  

git config user.email "ulag.india@gmail.com" - To update the email.  

git config --global user.name "Ulaganathan Vallinayagam" - To update the global user name.  
git config --global user.email "ulag.india@gmail.com" - To update the global email. 

git branch -b <branch_name> - To create a new branch.  
git clone -b "development" https://code.company.com/metricsapp/metrics-app.git  
git clone --branch release/Phase3_Day3 https://<username>@g<location>project.git - To clone from a specific branch.  
git checkout <branch_name> - To switch over to other branch.  

git reset --hard - To revert all your local changes.

git stash - To move your local changes to Hash.  
git stash pop - To bring back the changes to local from Hash.  

git merge <branch_name> - Go to the source branch and use this command to pull the latest contents from the destination branch.

git fetch origin - It will retrieve the remote branches so that we can git diff or git merge them with the current branch.

git pull origin <branch_name> - To pull the contents from other branch to local.  
git push origin <branch_name> - To push the contents to other branch to local.  

###### Merge Process
git checkout develop  
git pull  

git checkout master  
git pull  

git merge develop - To merge the contents from develop to master. 

** <<<<<<< HEAD - Current branch contents start here. ** 
** ======= - Differentiator of the contents between branches. **  
** >>>>>>> develop - Incoming branch contents ends here. ** 

git merge --abort - To abort the merge changes when MERGE_HEAD is present. 
git reset --merge ORIG_HEAD - To abort the merge changes when auto merge is completed. 

git log --oneline - To list the commit history with one line details. 

git revert commitid - To revert the changes. Need to git push to push the changes again. 

## Maven Commands

mvn clean install -DskipTests - To skip the test case execution.  
mvn spring-boot:run - To start the application from local command prompt.  
mvn clean install -P dev - To run the testcases with dev profile.  
