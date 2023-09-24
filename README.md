# Git & Github - Manual

Git is a distributed version control system that tracks changes in any set of computer files, usually used for coordinating work among programmers who are collaboratively developing source code during software development.

Github is a website that allows developers to store and manage their code using Git.

Configuring Git:

git config --global user.name "My name" <br>
git config --global user.email "myname@email.com" <br>
git config --list

<h1>Clone & Status:</h1>

clone - cloning a repository on our local machine

  git clone <-some link->

status - displays the state of the code

  git status

{untracked - new files that git doesn't track yet, modified - changed, staged - file ready to committed, unmodified - unchanged}

<h2>Add & Commit:</h2>

add - adds new or changed files in your working directory to the Git staging area

  git add <-file name->

commit - it is the record of change

  git commit -m "some message"
