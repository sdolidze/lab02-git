# Level 02 - Branch

## Step 1

`echo "Gold\nSilver\nBronze\n" > metals.md`

Create file `metals.md` with 3 lines: `Gold`, `Silver`, `Bronze`

`echo "Small\nMedium\nLarge\n" > sizes.md`

Create file `sizes.md` with 3 lines: `Small`, `Medium`, `Large`

`git init`

Initialize an empty git repository

`git add --all`

Add all **untracked** files to **staging**

`git commit -m "initial commit"`

Commit all **staged** files

## Step 2

`git checkout -b feat/add-metals`

Create branch `feat/add-metals` and switch to the branch

`echo "Gold\nSilver\nBronze\nAluminium\nTitanium\n" > metals.md`

Overwrite file `metals.md` with 5 lines: `Gold`, `Silver`, `Bronze`, `Aluminium`, `Titanium`

`git commit -am "add famous metals"`

Stage and commit all **staged** files

## Step 3

`git checkout master`

Move to `master` branch

`git checkout -b feat/remove-size`

Create branch `feat/remove-size` and switch to the branch

`git branch`

List all branches and show current one

`echo "Small\nLarge\n" > sizes.md`

Overwrite file `sizes.md` with 2 lines: `Small`, `Large`

`git commit -am "remove medium size"`

Stage and commit all **staged** files

## Step 4

`git checkout master`

Move to `master` branch

`git checkout -b feat/add-fruits`

Create branch `feat/add-fruits` and switch to the branch

`echo "Apple\Orange\n" > fruits.md`

Create file `fruits.md` with 2 lines: `Apple`, `Orange`

`git add --all`

Stage all **untracked** files

`git stash`

Save all staged files to temporary storage called **stash**

`git checkout master`

Move to `master` branch

`git checkout feat/add-fruits`

Move to `feat/add-fruits` branch

`git stash pop`

Move all files from **stash** to **staging** and apply to the file system

`git commit -m "add fruits"`

Commit all **staged** files

## Step 5

`git checkout master`

Move to `master` branch

`git branch -D feat/add-metals`

Delete `feat/add-metals` branch

`git branch -D feat/remove-size`

Delete `feat/remove-size` branch

`git branch -D feat/add-fruits`

Delete `feat/add-fruits` branch
