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
