### Notes on Git

Git is a DVCS (Distributed Version Control System) that allows users to take snapshots of their code and save them to the cloud. It's quick because it relies on local operations, while also providing change tracking and mitigating loss of data.

Handy commands:

command | description
:---: | ---
git help *(command)* | looks up help for a specific command
git clone *(repository link)* | clones an existing repository as a sub-directory to pwd
git status | checks for changes that require adding/committing
git add *(filename)* | adds file to tracking
git add * | adds all files to tracking
git commit -m "*(update description)*" | creates a commit with tracked files
git push origin master | pushes committed changes to the master branch in the cloud

[Return to table of contents](README.md)