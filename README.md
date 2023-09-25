# Git & Github - Manual

Git is a distributed version control system that tracks changes in any set of computer files, usually used for coordinating work among programmers who are collaboratively developing source code during software development.

Github is a website that allows developers to store and manage their code using Git.

Configuring Git:

git config --global user.name "My name" <br>
git config --global user.email "myname@email.com" <br>
git config --list

<h3>Clone & Status:</h3>

clone - cloning a repository on our local machine

&nbsp; git clone <-some link->

status - displays the state of the code

&nbsp; git status

{untracked - new files that git doesn't track yet, modified - changed, staged - file ready to committed, unmodified - unchanged}

<h3>Add & Commit:</h3>

add - adds new or changed files in your working directory to the Git staging area

&nbsp; git add <-file name-> <br>
&nbsp; git add . (dot adds all files at once)

commit - it is the record of change

&nbsp; git commit -m "some message"

<h3>Push Command:</h3>

push - upload local repo(laptop/pc) content to remote repo(github)

&nbsp; git push origin main

<h3>Init Command:</h3>

init -  used to create a new git repo

&nbsp; git init <br>
&nbsp; git remote add origin <-link->   <br>
&nbsp; git remote -v    (to verify remote)  <br>
&nbsp; git branch       (to check branch)   <br>
&nbsp; git branch -M main   (to rename branch)  <br>
&nbsp; git push origin main

&nbsp; git push -u origin main (-u meaans set upstream for push on the main branch only afterward)

<h3>WORKFLOW</h3>

&nbsp; Github Repo > clone > changes > add > commit > push

<h3>Git Branches:</h3>

&nbsp; git branch  (to check branch)   <br>
&nbsp; git branch -M main  (to rename branch)  <br>
&nbsp; git checkout <-branch name->    (to navigate)   <br>
&nbsp; git checkout -b <-new branch name->    (to create new branch)   <br>
&nbsp; git branch -d <-branch name->   (to delete branch)

<h3>Merging Code:</h3>

Way1:

&nbsp; git diff <-branch name->    (to compare commits, branches, files and more)  <br>
&nbsp; git merge <-branch name->   (to merge two branches)

Way2:

&nbsp; Create a pull request (which let you to tell others about the changes you've pushed to a branch in a Github Repository)

<h3>Pull Command:</h3>

pull - upload remote repo(github) content to local repo(laptop/pc)

&nbsp; git pull origin main

<h3>Undoing changes:</h3>

Case 1: staged changes
    
&nbsp; git reset <-file name-> <br>
&nbsp; git reset

Case 2: commited changes (for one commit)

&nbsp; git reset HEAD~1

Case 3: commit changes (for many commits)

&nbsp; git reset <-commit hash->    <br>   
&nbsp; git reset --hard <-commit hash->


 NOTE:

    git log (to check all commits history)

<h3>Fork:</h3>

A fork is a new repository that shares code and visibility settings with the original “upstream” repository.
