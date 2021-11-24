 # Git manual
 ### Always Check for repo status

 ````bash
 git status
 ````
 ### Show local branches

 ````bash
 # the branch you are on 
 # will be marked with *
 git branch
 ````

### Merge dev branch into your branch

 ````bash
 # pull updates from remote dev branch
 git switch dev
 git pull

 # merge dev branch into your branch
 git switch <your_branch>
 git merge dev
 ````


 ### Get a remote branch

 ````bash
 # fetch remote branch info
 git fetch origin <branch_name>:<branch_name>
 # switch to newly fetched branch
 git switch <branch_name>
 # pull any new updates to this branch
 git pull origin <branch_name>
 ````

 ### Push a local branch to remote

 ````bash
 # create a new local branch
 # and switch to it
 git switch -C <new_branch_name>
 # add files and commit to newly created branch
 git add .
 git commit -m "Add new_branch_name"
 # set new remote branch name to newly created local branch name
 git push -u origin <new_branch_name>
 ````
