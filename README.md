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
