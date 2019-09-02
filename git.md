# Ex. 
* Create a repository in github called SummerSchool
* Initialize your summerschool folder as a git repo (`git init`)
* add some files using the terminal (`git add ...`) 
* commit your changes with a meaningful commit message (`git commit -m "..."`)
* add remote origin (`git remote add origin git@................. `)
* push your changes to the remote repository (`git push origin master`)
## Initialize repo
 `git init`

## Add changes
 `git add file1.py file2.py`

 `git add *` <---- add all files

## Commit
 `git commit -m "Descriptive commit message"

## Pull remote changes to local repo
git will gonna pull remote changes and gonna try to merge the remote changes with yours

 `git pull origin master`

## Push local changes to remote repo
 `git push origin master`

Tip: Always pull for changes before push your changes

## Merge conflicts
If your local changes are in conflict with the remote one(i.e: both modified same line) you need to solve that conflict manually, how?
* Open the file
* Edit it with the final version
* Save the file
* `git add the_file.py`
* Commit the fix: `git commit -m "Fix merge conflict in the_file.py"`
* push the final version `git push origin  master`