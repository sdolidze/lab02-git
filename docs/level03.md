# Level 03 - Merge

## Setup

`git init`

`echo "Gold\n" > metals.md`

`git add --all`

`git commit -m "initial commit"`

## Add Aluminium

`git branch feat/add-metal-aluminium`

`git checkout feat/add-metal-aluminium`

`echo "Gold\nSilver\nBronze\nAluminium\n" > metals.md`

`git add --all`

`git commit -m "add aluminium"`

## Add Titanium

`git branch feat/add-metal-titanium`

`git checkout feat/add-metal-titanium`

`echo "Gold\nSilver\nBronze\nTitanium\n" > metals.md`

`git add --all`

`git commit -m "add titanium"`

## Merge aluminium without conflict (fast-forward)

`git checkout master`

`git merge feat/add-metal-aluminium`

`git branch -D feat/add-metal-aluminium`

## Merge titanium with conflict (manual merge)

`git merge feat/add-metal-titanium`

`git diff`

`echo "Gold\nSilver\nBronze\nAluminium\nTitanium\n" > metals.md`

`git add --all`

`git commit -am "fix merge conflict"`

`git branch -D feat/add-metal-titanium`

`git log`
