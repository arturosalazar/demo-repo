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
