This is my own Git cheat sheet. 

#### Commit changes + Create a new branch + Change to that branch + push changes

```bash
git status // Optional
git branch something/name_of_the_branch //creates the branch
git checkout something/name_of_the_branch  //swaps the current git to that branch
git status //Optional
git add .
git commit -m "Added some nice stuff"
git push --set-upstream origin something/name_of_the_branch
```

#### Use Master + get the latest

```bash
git checkout master //swpas to master branch
git fetch  //gets all the changes
git pull //pull the changes
```

#### Discard all the changes

```bash
git stash save --keep-index
git stash drop
```

#### Initialize the repo
```bash
git init //initialize the folder as a repo
git add .
git commit -m "First commit - your message goes here"
git remote add origin https://github.com/ACCOUNT_NAME/REPO_NAME.git
git push -u origin master //Or instead of master it can be the branch name
```

#### Some Git explained

Instead of using "." It can be a specific file as well

```bash
git —version
git init // initialize the folder as a repo
git add . // add all the files to staging 
git status  // returns what is in staging env and whats not added to working env
git log // see the logs for this repo
git checkout . // takes whatever is in staging and add it to work env
git reset HEAD . // takes out whatever is in staging
git commit -m “MESSAGE TO COMMIT” // commit changes
girl rm file // deletes a file in work and staging env
git add —all // adds everything also deletes stuff
git checkout HASH // takes whatever is in staging and put it in work env
git branch // show me the available branches
git checkout nameOfTheBranch // changes to another branch
git merge nameOfTheBranch // merges the current branch with the target one
git branch -m name1 newName  // change the name of the branch
git branch -D nameOfTheBranch  // Deletes the branch

```

#### Stuff to add to .gitignore file

```text
# Compiled source #
*.com
*.class
*.dll
*.exe
*.o
*.so

# Packages #
*.7z
*.dmg
*.gz
*.iso
*.jar
*.rar
*.tar
*.zip

# Logs and databases #
*.log
*.sql
*.sqlite

# OS generated files #
.DS_Store
.DS_Store?
._*
.Spotlight-V100
.Trashes
ehthumbs.db
Thumbs.db
```
