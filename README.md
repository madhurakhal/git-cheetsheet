# git-cheetsheet
Git commands cheet sheets. This document will be updated frequently.


### Seeing conflict files
`git diff --name-only --diff-filter=U`

### Pushing new branch and tracking it
`git push -u origin branch_name`

### Pulling new branch and set up track
`git checkout --track origin/branch_name`

### Resetting previous commit
`git reset HEAD~`

### adding all files with some extension
`git add *.ts (extension)`


### list all the remote branch
`git branch -r`

`git branch -a (all from local and remote)`


### renaming branch
`git branch -m <oldname> <newname>`

`git branch -m <newname>` (if you are in the branch)


### stashing in git
`git stash push -m "message"`

`git stash apply stash@{index}`

`git stash save "stash_name"`
`git stash pop stash@{stash_name}`


### showing remote branches
`git  show origin`

### showing all remote branches
`git branch -r`


### remove all merged branch
 `git branch --merged master | grep -v master | xargs -n 1 git branch -d` be careful you should be in master branch.



### To delete all branches on remote that are alread merged
`git branch -r --merged | grep -v master | sed 's/origin\///' | xargs -n 1 git push --delete origin`

### To delete all branch on local machine
`git branch | grep -v "master\|Release-02-2022\|feature-remove-any-types" | xargs git branch -D`
