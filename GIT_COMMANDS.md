## create a new repository on the command line
```
    echo "# credible" >> README.md
    git init
    git add README.md
    git commit -m "first commit"
    git branch -M main
    git remote add origin git@github.com:PyCloudWorld/credible.git
    git push -u origin main
```
## create a new branch from main by command line
```
git checkout main
git pull origin main
git checkout -b <new-branch-name>
```
## to list all local branches in your Git repository, use the following command:
```
git branch
```

## To fetch all data from the remote repository to your local repository, you can use the following command:

```
git fetch --all
```

## If you want to ensure that your local branches are also updated with the latest changes from the corresponding remote branches, you should use git pull for each branch or:

```
git pull --all
```

## To switch between branches in Git, you can use the git checkout command or the newer git switch command. Here are both methods:

```
git checkout branch-name
```

## Replace branch-name with the name of the branch you want to switch to.

Using git switch (recommended):
```
git switch branch-name
```

## If the branch you want to switch to does not exist locally but does exist on the remote, you can create and switch to it in one step using:

```
git switch -c branch-name --track origin/branch-name
```