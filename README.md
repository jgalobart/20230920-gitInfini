# Commands 

## Pull get the latest version of the project
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

## Push push the changes to the remote repository
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


# -------------------- TAG ---------------------------

## Tag commit already done with a version name (v1.0), when pushing will be uploaded automatically
```bash
    git tag V1.0 (for exemple)
```

# -------------------- PRIVACY CONTROL (DO NOT INSERT FILES IN REPOSITORY) ---------------------------

Create a .gitignore with each file to do not include in a line
All files starting with a --> a*
All files ending with jpg --> *.png
All files in a folder --> FolderName/


