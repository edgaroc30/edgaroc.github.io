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
