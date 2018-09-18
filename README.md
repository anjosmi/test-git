# test-git
Learning git one commit at a time...

# Overview: Why do we need version control system? 
To be able to record changes to a project or file over time so that you are able to recall specific version later.

# Creating a repository
DEMO in GitHub

# Basic commits
<table class="tg">
  <tr>
    <th class="tg-yw4l"><b>Code</b></th>
    <th class="tg-yw4l"><b>Description</b></th>
  </tr>
  <tr>
    <td class="tg-yw4l">git clone https://github.com/anjosmi/test-git.git</td>
    <td class="tg-yw4l">Clone a copy of the latest version for test-git repo master using https</td>
  </tr>
  <tr>
    <td class="tg-yw4l">git remote set-url origin https://github.com/anjosmi/test-git.git</td>
    <td class="tg-yw4l"></td>
  </tr>
  <tr>
    <td class="tg-yw4l">git branch</td>
    <td class="tg-yw4l">Tells you which branch you are working at the moment</td>
  </tr>    
  <tr>
    <td class="tg-yw4l">git clone git@github.com:anjosmi/test-git.git</td>
    <td class="tg-yw4l">Clone a copy of the latest version for test-git repo master using SSH</td>
  </tr>
  <tr>
    <td class="tg-yw4l">git commit -m "describe your commit"</td>
    <td class="tg-yw4l">Commit change in your local repo</td>
  </tr>
  <tr>
    <td class="tg-yw4l">git status</td>
    <td class="tg-yw4l">Check the state of your files</td>
  </tr>
  <tr>
    <td class="tg-yw4l">git log</td>
    <td class="tg-yw4l">Use to display the history of commits</td>
  </tr>
  <tr>
    <td class="tg-yw4l">git fetch [remote-name]</td>
    <td class="tg-yw4l">Fetch the remote data into your local repo (e.g. git fetch origin)</td>
  </tr>  
  <tr>
    <td class="tg-yw4l">git pull origin master</td>
    <td class="tg-yw4l">Check for changes on our GitHub repository and pull down any new changes</td>
  </tr>  
  <tr>
    <td class="tg-yw4l">git config --list</td>
    <td class="tg-yw4l">Check your settings</td>
  </tr>  
  <tr>
    <td class="tg-yw4l">git push [remote-name] [branch-name]</td>
    <td class="tg-yw4l">Push your code to a remote repo (e.g. git push origin master or git push origin featureX)</td>
  </tr>  
  <tr>
    <td class="tg-yw4l">git checkout -b <branch name></td>
    <td class="tg-yw4l">Create a branch with given name</td>
  </tr> 
  <tr>
    <td class="tg-yw4l">git branch -d <branch name></td>
    <td class="tg-yw4l">Delete branch with given name. Make sure you are in master before you run the command to delete a certain branch</td>
  </tr>  
  <tr>
    <td class="tg-yw4l">git checkout -- file.txt</td>
    <td class="tg-yw4l">This will remove all the changes applied to file file.txt since last commit</td>
  </tr> 
  <tr>
    <td class="tg-yw4l">git reset HEAD file.txt</td>
    <td class="tg-yw4l">Unstage your change</td>
  </tr>   
  <tr>
    <td class="tg-yw4l">git checkout -- <name of the file></td>
    <td class="tg-yw4l">Undo changes that were not committed yet</td>
  </tr>    
</table>

# Branching / merging / pull requests

    Step 0: Bring in the changes
    git fetch origin
    
    Step 1: Create a branch
    git checkout -b improve-test
    
    Step 2: Check different branches
    git branch
    
    Apply a change!!! 

    Step 3: Make sure the branch is up to date
    git merge master

    Step 4: Merge the changes and update the server
    git checkout master
    git merge improve-test
    git push origin master
  

# Git flow or GitHub flow
https://lucamezzalira.com/2014/03/10/git-flow-vs-github-flow/


