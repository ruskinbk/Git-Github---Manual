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