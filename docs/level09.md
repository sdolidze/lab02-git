#Questions

## How to unstage a file?

`$ git reset`

## How to delete a file?

`$ git rm <file>`

`$ git rm --cached <file>`

## How to undo a commit locally?

`$ git reset --hard HEAD~1`

Current `HEAD` becomes `HEAD~1` (previous commit)

## How to undo a commit remotely?

`$ git reset --hard HEAD~1`

Current `HEAD` becomes `HEAD~1` (previous commit)

`$ git push -f`

Always be **extra** careful when force pushing

## How to create a branch from a commit?

`$ git checkout -b <branch> <commit>`

## How to rest to a particular commit?

`$ git reset --soft (maintain local structure)`

`$ git reset --hard (overwrite)`

## How to reset a particular file to a snapshot?

`$ git reset <commit> <file>`

## How to delete a branch locally?

`$ git branch -d <branch>`

## How to delete a branch remotely?

`git push origin --delete <branch>`

## How to diff two commits?

`git diff <commit> <commit>`

## How to doff two files?

`git diff <commit>:<file> <commit>:<file>`
