# Commands 

## Pull get the latest version of the project (will do the pull of the all the branches)
```bash
    git pull
```

## Add add the files to the staging area
```bash
    git add <file>
```

## Commit commit the changes to the local repository
```bash
    git commit -a -m "message"
```

## Push push the changes to the remote repository (push only of the branch you are in, if does not exist in production will ask to create it)
```bash
    git push
```

## Status check the status of the repository
```bash
    git status
```


# -------------------- GIT STASH ---------------------------

## Stash go to the last commit version
```bash
    git stash
```

## Return to the version of the moment when we did the last git stash and remove it from memory
```bash
    git stash pop
```

## See all the versions stashed 
```bash
    git stash list
```

## Return to the version of the moment when we did the specified git stash and remove stash from memory
```bash
    git stash pop stash@{IDStash->found in git stash list}
```

## Return to the version of the moment when we did the specified git stash but mantain it in memory
```bash
    git stash apply stash@{IDStash->found in git stash list}
```

# -------------------- BRANCHES ---------------------------

## Create new branch with all the working content saved (have to commit new saves after too)
```bash
    git checkout -b BranchName
```

## Move to existing branch (non commited changes will be moved to the branch too)
```bash
    git checkout  BranchName
```

## Merge current branch with other branches (se when addign fucntionalities to master, move there and do merge) CNTRL SHIFT M
```bash
    git merge  BranchName
```

## See all branches
```bash
    git branch
```


# -------------------- TAG ---------------------------

## Tag commit already done with a version name (v1.0), when pushing will be uploaded automatically. Usually done in master
```bash
    git tag V1.0 (for exemple)
```

# -------------------- PRIVACY CONTROL (DO NOT INSERT FILES IN REPOSITORY) ---------------------------

Create a .gitignore with each file to do not include in a line
All files starting with a --> a*
All files ending with jpg --> *.png
All files in a folder --> FolderName/

# -------------------- GIT FLOW ---------------------------

READ http://datasift.github.io/gitflow/IntroducingGitFlow.html


# ------------------------CI / CD---------------------------
It is possible to have automatisms to upload a project to production.
Automation tests to check web will be OK at production
Github actions to do some automativ actions that need to be done always when uploading the project to production (python manage.py etc)