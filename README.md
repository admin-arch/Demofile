# Prerequisite
To install jenkins with jenkins.war file
To install apache tomcat server-9
To create Github account
To Download Git
Create sample Hello World java code in local machine

# Workflow
Open Git Bash
Navigate to directory-> mkdir<folder name>
  Type the following commands:
  git init (to initialise)
  git add "FirstProgram.java"  (to add all the relevant files)
  git status (to check the status of the file whether it is commited)
  git commit -m "First Commit" (to add file from staging area to local repo)
  
# Connect it to Github
Go to Github
log in to the account
click the new repository button at the top right and create new remote repo(with Public and add Readme file), copy the remote repo URL
Go to Git
  git remote add origin "remote repo URL"
  git push "remote repo URL" (Push FirstProgram.java from local repo to remote repo)
  git pull "remote repo URL" (Pull files from remote repo to local repo)
  git checkout -b "branchname" (creates new branch in Github)

# Open Jenkins
Add github plugins (Go to Manage Jenkins->Manage Plugins->Available->Github Plugin->Submit)
Create New item (Go to New item->item name (FirstProgram.java) ->type of project (freestyle)->add)
Go to (Source code mamagement->git)
Paste repo URL from Github containing FirstProgram.java (keep master as default branch)
Go to build to give compile instruction (command->java FirstProgram.java->add)
Save the Project
Click on build, if program builds successfully(SUCCESS) else(FAILURE)

# Steps to Run Jenkins on Tomcat Server
Open Tomcat folder extract all the files goto bin->startup (run startup windows bat file to launch the tomcat server)
Copy the jenkins.war file to the subfolder webapps in the Tomcat installation it will autogenerate a jenkins folder
Go to the url "http://localhost:8080/jenkins" to launch the initial jenkins page on the Tomcat server



  
  




