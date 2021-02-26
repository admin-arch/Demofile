# Prerequisite
1. To install jenkins with jenkins.war file
2. To install apache tomcat server-9
3. To create Github account
4. To Download Git
5. Create sample Hello World java code in local machine

# Workflow
1. Open Git Bash




   ![1](https://user-images.githubusercontent.com/79540238/109284224-a3bbc300-7845-11eb-803d-17ef7da0b802.PNG)

2. Navigate to directory-> mkdir->folder name
  ### Type the following commands:
  1. git init (to initialise)


     ![2](https://user-images.githubusercontent.com/79540238/109284230-a4ecf000-7845-11eb-802a-449ca5094142.png)
  3. git add "FirstProgram.java"  (to add all the relevant files)



     ![3](https://user-images.githubusercontent.com/79540238/109284232-a5858680-7845-11eb-8918-4fca5f697ea9.PNG)
  5. git status (to check the status of the file whether it is commited)



     
     ![4](https://user-images.githubusercontent.com/79540238/109284788-3f4d3380-7846-11eb-8f9c-632833cbe2da.PNG)
  7. git commit -m "First Commit" (to add file from staging area to local repo)


     
     ![5](https://user-images.githubusercontent.com/79540238/109284789-407e6080-7846-11eb-86c3-d997ee88ca5c.PNG)
  
## Connect it to Github
1. Go to Github
2. log in to the account
3. click the new repository button at the top right and create new remote repo(with Public and add Readme file), copy the remote repo URL



   ![6](https://user-images.githubusercontent.com/79540238/109284790-4116f700-7846-11eb-930c-6a02a78c7f42.PNG)
5. Go to Git
  1. git remote add origin "remote repo URL"
  2. git push "remote repo URL" (Push FirstProgram.java from local repo to remote repo)
  3. git pull "remote repo URL" (Pull files from remote repo to local repo)
  4. git checkout -b "branchname" (creates new branch in Github)

## Open Jenkins
1. Add github plugins (Go to Manage Jenkins->Manage Plugins->Available->Github Plugin->Submit)
2. Create New item (Go to New item->item name (FirstProgram.java) ->type of project (freestyle)->add)
3. Go to (Source code mamagement->git)
4. Paste repo URL from Github containing FirstProgram.java (keep master as default branch)
5. Go to build to give compile instruction (command->java FirstProgram.java->add)
6. Save the Project
7. Click on build, if program builds successfully(SUCCESS) else(FAILURE)

## Steps to Run Jenkins on Tomcat Server
1. Open Tomcat folder extract all the files goto bin->startup (run startup windows bat file to launch the tomcat server)
2. Copy the jenkins.war file to the subfolder webapps in the Tomcat installation it will autogenerate a jenkins folder
3. Go to the url "http://localhost:8080/jenkins" to launch the initial jenkins page on the Tomcat server




  
  




