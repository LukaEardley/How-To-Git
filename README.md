# How To Set Up A Git Repository


## Creating a new repository

1. Open GitHub
2. Go to Your Repositories
3. Click New Repository
4. Enter a name 
5. Choose access type of public/private
6. Tick the box to initialize the repository with a README
7. Use thr dropdown to add a .gitignore for either the language or IDE you are using (.NET or Visual Studio for example)

## Cloning the repository

1. Make sure you have gitbash installed
2. Navigate to the directory you want to clone the repository to
3. Right click and select open gitbash here (inside the folder you want the repository in)
4. On GitHub navigate to the repository and there should be a green button calle "clone or download"
5. Copy the link in the box under the headding "clone with HTTPS"
6. In the gitbash terminal execute the command `git clone <the-link-you-just-coppied>`
7. The repository should now be cloned

## Checkout a branch

1. Use the command `git checkout <branch-name>` to checkout the branch and allow your self to make changes to it

## Create a new branch from master

1. Make sure gitbash has the text (master) next to the directory you are in in the terminal
2. use the command `git checkout -b <the-name-of-the-branch-you-want-to-make>`
3. You should now have a new branch with a copy of the code that is in master for you to be able to make changes to

## Check for changes on a branch

1. Use the command `git status` to see a list of the files you may have changed.
2. Red file paths are files you have changed
3. Green file paths are files that are new and have been added to the repository

## Committing you code

1. Use the command `git add .` to stage oall the files to be commited
2. Now use the command `git comnmit -m "<the-commit-message-you-want>"`

#### As an alternative the aforementioned commands can be combined into a single command

1. Use the command `gitl
