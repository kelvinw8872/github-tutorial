# **GitHub Tutorial**

_by Kelvin Wang_

---
## Git vs. GitHub
**Git** is a version-control that keeps track of your code and lets you manage it. **GitHub** is a cloud that stores your code. It acts as a host which you can use to share and collaborate with others!



---
## Initial Setup
1. make a github account
2. [Follow these directions](https://github.com/hstatsep/ide50/blob/master/README.md)  
    * the SSH key is used to clone other peoples code to make it your own! We use SSH instead of HTTP because you have to log into your github everytime with HTTP

---
## Repository Setup
1. create a repository on github.
2. go to your IDE and create a repository!
3. CD into it then `git init` to intitialize git.
4. Whenever you make a change do `git add .` This will add the changes to the stage.
5. After adding you can commit it by doing `git commit -m "<commit message>"` This will save the changes made 
---
## Workflow & Commands
`git init` is used to turn the directory you want into a repository. This should only be done once in the beginning. It intializes git in our directory for version-control.   


`git add .`  will add all of your current work to the stage. This keeps track of all changes made.  


`git commit -m ""` will take a snapshot of the files on the stage. This saves you work to the local repository.  


`git status` is used to keep track of your work. It displays all changes made so you can see if everything is alright. It can also be used to find errors in code for you to fix. 

    * While coding make sure to use git status to make sure there are no errors and everything is working. Add and commit while making changes and push when you feel it is ready. 

---
## Rolling Back Changes
* If you want to undo an edit in your ide, use git status. It will tell you how to undo this. 
* `git checkout -- <file>...` is used to undo changes in the directory you are working in.
* `git reset HEAD <file>` is used to unstage something/undo an add.
* `git reset HEAD^ <file>` is used to uncommit something.
* To un-push use `git push -f origin HEAD^:master` This will undo the git push!