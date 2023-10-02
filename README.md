# Demo Repo

This is a demonstration repo to practice git

## Step-by-step guide to add an existing Git repository from your computer to GitHub

### On Github:
    []Create New Repository (Log into account and click on the "+" icon)
    []Fill in your repository name and description and whether the repo is public or private
    []Do NOT initialize your repo with a README, .gitignor, or license (since you are using an existing repo)
    []Click "Create repository"


### On Computer - In Terminal:
    []Navigate to existing git repository on your computer
    []Use git init (just to double check you do have the repository initialized)
    []Add Your GitHub Repository as a Remote:
        []After creating the new repo on GitHub, you'll see a URL for it. Copy that URL.
        []Run the following: git remote add origin YOUR_COPIED_GITHUB_URL
    []Push Your Code to github
        []Pull any changes (good practice to ensure no conflict)
            []Run the following: git pull origin main --allow-unrelated-histories
        []Push your code
            []Run the following: git push -u origin main


## F.A.Q
* What is the meaning behind the command: git remote add origin YOUR_COPIED_GITHUB_URL
    * git: command-line tool to work with a git repo
    * remote: specifies we are working with 'remote' repositories - version of your project hosted somewhere other than your local machine
    * add: tells git we want to add a new remote
    * origin: conventional name for the default remote repo. Just a shorthand for the remote repo URL (you can name it something else, origin is the convention)
    * YOUR_COPIED_GITHUB_URL: Replace this with the URL to the git repo you've created on GitHub. It is the address that your local repository will use to push and pull from.

    tl;dr - establishes a connection between your local repository and the remote repository on GitHub, setting up a path to push/pull between the two

* What is the meaning behind the command: git push -u origin main
    * git: command-line tool to work with a git repo
    * push: command to push changes from a local repository to a remote one
    * -u (or --set-upstream): link your local branch to corresponding remote branch in the remote repository. You only need to use this once because it will set the upstream branch for future 'git push' or 'git pull' commands
    * origin: conventional name for the default remote repo. Here, it is the name of the remote repository that you are pushing to. Just a shorthand for the remote repo URL 
    * main: The name of the branch you are pushing. 

    tl;dr - pushes your local changes in the "main" branch to the "main" branch of the "origin" remote repository and sets that remote branch as the upstream for your local "main" branch

* What is the meaning behind the command: git pull origin main --allow-unrelated-histories
    * git: command-line tool to work with a git repo
    * pull: command to fetch ("pull") changes from a remote repository to your local welcome branch and merge those changes into your local branch (combo of 'git fetch' and 'git merge'
    * origin: conventional name for the default remote repo. Here, it is the name of the remote repository that you are pushing to. Just a shorthand for the remote repo URL
    * main: The name of the branch you are pushing.
    * --allow-unrelated-histories: This option is a bit special and is not typically required for regular git pull operations. You'd use this option when you're trying to merge two branches that started off with unrelated commit histories
