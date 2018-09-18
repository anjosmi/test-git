# test-git

Learning git one commit at a time...

# Why do we need version control system?
To be able to record changes to a project or file over time so that you are able to recall specific version later.

# High level overview


# Creating a repository
DEMO in GitHub

# Basic commits
/***
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
    <td class="tg-yw4l">git clone git@github.com:anjosmi/test-git.git</td>
    <td class="tg-yw4l">Clone a copy of the latest version for test-git repo master using SSH</td>
  </tr>
</table>
***/

# Branching / merging / pull requests

Step 1: Bring in the changes and test
git fetch origin
git checkout -b improve-test origin/improve-test

Step 2: Make sure the branch is up to date
git merge master

Step 3: Merge the changes and update the server
git checkout master
git merge improve-test
git push origin master


# Git flow or GitHub flow

https://lucamezzalira.com/2014/03/10/git-flow-vs-github-flow/


