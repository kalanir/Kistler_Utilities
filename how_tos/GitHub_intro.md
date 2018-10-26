# Intro to GitHub

## I want to create a new repository

## I want to clone a repository
Cloning means:

## I want to make changes to a repository locally, and push them to my origin/master repository

- `git status`: will tell you if there are files/ file changes in your working directory that have not been committed to your repository
- `git add .`: start adding changes to the repository. You can add specific files but replacing . with the file. to undo this, `git reset` will undo changes
- `git status`: will tell you if changes have been staged - currently a git add does not make permanent changes
- `git commit -m "any message"`: commit these changes to your repository
- `git status`: at this point it should say your working directory is clean

example workflow:
```
➜  Kistler_Utilities git:(master) git status
On branch master
Your branch is up-to-date with 'origin/master'.
Untracked files:
  (use "git add <file>..." to include in what will be committed)

	how_tos/

nothing added to commit but untracked files present (use "git add" to track)
➜  Kistler_Utilities git:(master) ✗ git add .
➜  Kistler_Utilities git:(master) ✗ git status
On branch master
Your branch is up-to-date with 'origin/master'.
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

	new file:   how_tos/JupyterNotebook_onAWS.md
	new file:   how_tos/RStudio_onAWS.md
	new file:   how_tos/Reflow_basic.md

➜  Kistler_Utilities git:(master) ✗ git commit -m "new files"
[master 229d4f2] new files
 3 files changed, 179 insertions(+)
 create mode 100644 how_tos/JupyterNotebook_onAWS.md
 create mode 100644 how_tos/RStudio_onAWS.md
 create mode 100644 how_tos/Reflow_basic.md
➜  Kistler_Utilities git:(master) git status
On branch master
Your branch is ahead of 'origin/master' by 1 commit.
  (use "git push" to publish your local commits)
nothing to commit, working tree clean
➜  Kistler_Utilities git:(master) git push
Counting objects: 6, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 3.51 KiB | 3.51 MiB/s, done.
Total 6 (delta 0), reused 0 (delta 0)
To https://github.com/kalanir/Kistler_Utilities.git
   9e7c37b..229d4f2  master -> master
➜  Kistler_Utilities git:(master) git status
On branch master
Your branch is up-to-date with 'origin/master'.
nothing to commit, working tree clean

```



## I want to make a branch off of a repository, and make changes, and push that branch

## I want to merge my branch to origin/master