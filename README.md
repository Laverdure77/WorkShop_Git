# WorkShop_Git

Basic demo: git flow to setup a new project.  
Team 📊 AI BeCode 📈


[VS CODE documentation](https://code.visualstudio.com/docs/sourcecontrol/overview)

[Github documentation](https://docs.github.com/en/get-started/importing-your-projects-to-github/importing-source-code-to-github/adding-locally-hosted-code-to-github#adding-a-local-repository-to-github-using-git)


# From github : clone

### 1. init empty repo from github and clone it using terminal


```bash
# create new empty repo on GitHub: top left github logo, home page
# to avoid errors, do not initialize _README_, license, # or `gitignore` files. 
# copy url from Quick Setup

# create a local folder for your new project
# open terminal in the new folder

git clone <REMOTE URL> 

# create a new main.py file

git add .
git commit -m "First commit, init repo"

git push -u origin main  # shorthand for git push --set-upstream origin main

git status

```


### 2. clone repo in vscode source control

	From source control panel in VS Code


# From local folder : init
	( empty or already populated )


### 1. init repo from terminal

```bash
# working directory = local project
git init -b main   # creates .git hidden folder in your project folder
                   # set name of MASTER branch 
                  
                  
git add .          # if already populated
git commit -m "First commit, init repo"

# git push would give fatal error because no remote repo specified yet 
# create new empty repo on GitHub: top left github logo, home page
# copy url from Quick Setup

git remote add origin <REMOTE URL>   # paste url, sets the new remote
git remote -v                        # check remote is set

git push -u origin main  # first time, to make sure to push from main to origin/main

git status               # You are good to go!! 😁

```

### 2. init repo from vscode source control

	From source control panel.
