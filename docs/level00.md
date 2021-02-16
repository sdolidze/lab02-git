# Level 00 - Commit

## Step 1

`git init`

File system has `.git` folder in the current directory

Git is initialized, but empty

### FS

```

```

### Git Staging

```

```

### Git Repository

```

```

## Step 2

`echo "Hello World" > README.md`

README.md is an **untracked** file for git (does not exist for git)

`git status`

### FS

```
- README.md
```

### Git Staging

```

```

### Git Repository

```

```

## Step 3

`git add README.md`

README.md file is **staged**, but not **committed**

`git status`

All **staged** changes will be part of the next **commit**

### FS

```
- README.md
```

### Git Staging

```
- README.md
```

### Git Repository

```

```

## Step 4

`git commit -m "initial commit"`

README.md file is now **committed**, you can always go back in time to see this version.

All **commits** are always saved locally on your computer.

### FS

```
- README.md
```

### Git Staging

```

```

### Git Repository

```
+ initial commit
  - README.md
```

## Step 5

`echo "const x = 5;" > index.js`

Creating file named `index.js`

`git add index.js`

You have to **stage** a file until you can commit it.

`git commit -m "add index file"`

index.js file is now **committed** with a unique **commit hash**. You can always go back in time to see this version.

`git status`

All **commits** are always saved locally on your computer.

### FS

```
- README.md
- index.js
```

### Git Staging

```

```

### Git Repository

```
+ initial commit
  - README.md
+ add index file
  - index.js
```
