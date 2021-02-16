# Level 01 - Versioning

## Step 1

HINT: run `git status` after each **git** command

`echo "Apple\nOrange\nPear\n" > fruits.md`

Create file `fruits.md` with 3 lines: `Apple`, `Orange`, `Pear`

`echo "Red\nGreen\nBlue\n" > colors.md`

Create file `colors.md` with 3 lines: `Red`, `Green`, `Blue`

`git init`

Initialize an empty git repository

`git add --all`

Add all **untracked** files to **staging**

`git commit -m "initial commit"`

Commit all **staged** files

## Step 2

`echo "Apple\nMango\nOrange\nPear\nKiwi\n" > fruits.md`

Overwrite file `fruits.md` with 5 lines: `Apple`, `Mango`, `Orange`, `Pear`, `Kiwi`

`git diff`

Compare state of the file system with the previous **commit**

`echo "Red\n\nBlue\nOrange\n" > colors.md`

Overwrite file `colors.md` with 3 lines: `Red`, `Blue`, `Orange`

`git diff`

Compare state of the file system with the previous **commit**

`git commit -am "update fruits and colors"`

Stage all **tracked** files (`-a`) and **commit** them

## Step 3

`echo "Cherry\nStrawberry\n" > fruits.md`

Overwrite file `fruits.md` with 2 lines: `Cherry`, `Strawberry`

`git diff`

Compare state of the file system with the previous **commit**

`git commit -am "reset list of fruits"`

Stage all **tracked** files (`-a`) and **commit** them

`git diff HEAD:fruits.md HEAD~2:fruits.md`

Compare current state of `fruits.md` with the state 2 commits ago

## Step 4

`rm fruits.md`

Delete `fruits.md` file

`git commit -am "remove fruits"`

Stage changes and commit them

`git checkout HEAD~1 fruits.md`

Restore state of `fruits.md` from previous commit

## Step 5

`mv fruits.md super-fruits.md`

Rename `fruits.md` to `super-fruits.md`

`git add --all`

Stage all changes

`git commit -m "rename fruits"`

Commit all staged files
