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


### showing remote branches
`git checkout show origin`
