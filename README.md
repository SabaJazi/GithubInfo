# Demo
a short abstract from this tutorial:
https://youtu.be/RGOj5yH7evk
## Creating a Repository in Github
1. sign in to github account.
2. on the first page, click on "+" sign on top right, choose "New Repository".
3. give a name for your repository in "Repository name" box.
4. choose either private or public for your repository(if private, only you and other contributors can see it).
5. click on "create repository" button.

## Using Git on Local machine
### Windows
If git is not already installed, follow this tutorial: https://www.atlassian.com/git/tutorials/install-git
1. click on "Install Git on Windows"
2. when you download the Git Windows installer, it is recommended to choose "Git Bash" option from the install menue(to have an easier time).
### Mac
If you are using a mac or linux operating system, you should already have it installed. You can check it this way:
1. open terminal application
2. type "git --version" (do not include " and notice space before -)
3. it should output the git version
4. if git is not already installed, follow this tutorial: https://www.atlassian.com/git/tutorials/install-git
5. it gives you few options for install, but Homebrew package manager is recommended.
## Set up in code editor
You can choose whatever code editor you prefer. We will cover a few of them in the following steps.
### VS Code
Visual Studio Code is a free code editor made by Microsoft and is widly used. You can install it free from https://code.visualstudio.com/
It is available on every major operating system.
1. first create your repository(folder) in your local drive.
2. If you want to mange your code in conda environments, go to "Anaconda installation".
3.
### Anaconda installation
1. Download anaconda or miniconda installer from this website : https://docs.anaconda.com/anaconda/install/
2.
# Important commands 
## git status
check the see the changes (change in code, new files,...)
The files names will be in red(or orange) in VScode
## git add 
you need to add something after "add". in most cases we use "." because we want to add all the changes.
so it will look like this: "git add ."
After entering this line, those file names will turn green and saved in local repository.
## git commit -m -m
to let the git know about your changes and updates, you run this command with first -m for commit title and second -m for optional description of commit(you can skip the second one)
## git push origin branch
to update the remote repository(aka github)
you have to declare the origin and the branch you are pushing to. after running this command you can refresh and see changes in github repository.

## git checkout
it is used to switch between branches.for example you can switch to main branch this way:
    git checkout main
You can create a new branch with it also by giving it the parameter -b. for example:
    git checkout -b feature-readme-instructions
after creating the branch you will be automaticly move to the new branch

## git reset
to undo the last thing you did.
for example if we mistakenly stage the readme.md file, to undo that we use this command:
git reset readme.md
(git reset will work too, it undos all last changes, but using the file name only undos that file)
to undo a commit, we use
git reset HEAD( HEAD is the pointer to the last commit)
If we use 
git reset HEAD~1
it points to a on step further than the commit and reset from that point.for example here, it will unstage the readme.md
if you want to undo a specific commit staging, there is no straight forward way to find that commit. 
What we do, is to see the log of commits using this command:
## git log
they will be listed as reversed chronological order.(the lasred will be shown first)
the commits are known to git with a unique hash. So we can copy the hash of the commit we want to go back to and use git reset with that.
to make the lsit of logs shorter we can use, 
git log --oneline
## git diff branch-name
to show the differences between what is in the branch and what you have changed.

## git fetch
to see the latest update on remote repository. It shows 1 to last commit id to the last commit id change and the branch it was done.
if the last commit id in fetch is not the last id in git log output, then it means the remote repository is some commits ahead of local.

## git pull origin branch-name
to update our local branch with the remote branch, we use pull command.
!Notic: make sure you have commited and pushed what you have done before that, or do the pull commit before any changes, because it can cause conflict if pushing to the same branch.

## how to pull a repository from github to your local system
first, in vscode, if terminal window is not open, click on view--> terminal to open it.
Then, using command "git clone" we will clone the repository on our machine.
