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

1. Use the command `git commit -am "<the-commit-message-you-want>"`

## Pushing your code to GitHub

1. Use the command `git push` to push the changes on a branch to GitHub

## Pushing a new branch of code to GitHub

1. If you try to push a branch to GitHub that only exists on your comnputer then gitbash will recommend the command `git push --set-upstream origin <the-name-of-your-branch>`.
2. Just use this command as it is the only way to push your new branch to GitHub

## Pulling code 

1. If the branch you have exists on your computer then make sure that branch is checked out and use the command `git pull` to pull the new changes of that branch to your computer.
2. If the branch you want only exists on GitHub and not on your computer then use the command `git fetch`. This will fetch all new branches and it does not matter what branch you have checked out when you use this command.
3. You will now be able to checkout the branch that just got fetched from GitHub

##### If you have made changes to a branch accidentally and need to pull or push or checkout another branch you can use the command `git reset --hard`. This will discard any changes made to that branch. Only use this command if you did not want to keep the changes you made.

##### If you try to checkout a different branch or push/pull on a branch with changes gitbash will not let you do this until you have decided what to do with them. Either commit your code before doing this or reset the branch as stated above ONLY IF YOU WANT TO DISGARD THOSE CHANGES


