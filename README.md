# Demo
Some description will be added later
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
