# GIT CHEAT SHEET
## Feature Branch Example

```
// if using develop, use that instead of master
git checkout master
git branch feature-task1
git checkout feature-task1

// make some changes

git add .
git commit -m "Changes..."

// when you're done with the feature
git push origin feature-task1

// pull any changes from master
git pull origin master
// merge master into your feature-task1 branch
git merge --no-ff master

// resolve conflicts, if any
// this may require git add & git commit

// switch back to master and merge changes
git checkout master
git merge --no-ff feature-task1
git push origin master

// delete old branches
// ONLY after they have been merged
git branch -d feature-task1
```

## Other Commands
```
// list branch you are on
git branch

// list all branches
git branch -a

// 'soft' pull
git fetch

// show status
git status

// undo commit (save changes)
git reset --soft HEAD~1

// undo commit (discard changes)
git reset --hard HEAD~1

// unstage file
git reset <commit> -- <path>

// unstage all files
git reset
```
