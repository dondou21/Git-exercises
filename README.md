# Git Project

The exercises to get good level in Git
# Bundle 1
# Exercice 1

```bash

## Initialization of git

PS C:\Users\DONDOU\Desktop\Git_Exercise> git init
Initialized empty Git repository in C:/Users/DONDOU/Desktop/Git_Exercise/.git/

No commits yet

nothing to commit (create/copy files and use "git add" to track)

## Renaming the  branch from Master to Main

PS C:\Users\DONDOU\Desktop\Git_Exercise> git branch -M main
PS C:\Users\DONDOU\Desktop\Git_Exercise> git status
On branch main


## Adding README.md and commit changes

PS C:\Users\DONDOU\Desktop\Git_Exercise> git status
No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)

nothing added to commit but untracked files present (use "git add" to track)
On branch main


Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   README.md

PS C:\Users\DONDOU\Desktop\Git_Exercise> git add REAME.md
fatal: pathspec 'REAME.md' did not match any files
PS C:\Users\DONDOU\Desktop\Git_Exercise> git add REAMDE.md
PS C:\Users\DONDOU\Desktop\Git_Exercise> git add README.md
PS C:\Users\DONDOU\Desktop\Git_Exercise> git commit -m 'init project'
[main (root-commit) 3d99a12] init project
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 README.md


## Creating Github repo and connect it with my project

PS C:\Users\DONDOU\Desktop\Git_Exercise> git add origin https://github.com/dondou21/Git-exercises.git
PS C:\Users\DONDOU\Desktop\Git_Exercise> git remote add origin https://github.com/dondou21/Git-exfatal: The current branch main has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin main

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

## Pushing My changes t Github

PS C:\Users\DONDOU\Desktop\Git_Exercise>  git push --set-upstream origin main
Counting objects: 100% (3/3), done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/dondou21/Git-exercises.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.
PS C:\Users\DONDOU\Desktop\Git_Exercise> git push 
Everything up-to-date
PS C:\Users\DONDOU\Desktop\Git_Exercise>

## Creating a new branch dev

PS C:\Users\DONDOU\Desktop\Git_Exercise> git checkout -b dev
PS C:\Users\DONDOU\Desktop\Git_Exercise> git status
On branch dev
nothing to commit, working tree clean
PS C:\Users\DONDOU\Desktop\Git_Exercise> git push 
fatal: The current branch dev has no upstream branch.
To push the current branch and set the remote as upstream, use


upstream, see 'push.autoSetupRemote' in 'git help config'.
PS C:\Users\DONDOU\Desktop\Git_Exercise> git push origin dev
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote:
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/dondou21/Git-exercises/pull/new/dev
remote:
To https://github.com/dondou21/Git-exercises.git
 * [new branch]      dev -> dev

## Creating from dev another branch test

PS C:\Users\DONDOU\Desktop\Git_Exercise> git checkout -b test
Switched to a new branch 'test'
PS C:\Users\DONDOU\Desktop\Git_Exercise> git push origin test
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote:
remote: Create a pull request for 'test' on GitHub by visiting:
remote:      https://github.com/dondou21/Git-exercises/pull/new/test
remote:
To https://github.com/dondou21/Git-exercises.git
 * [new branch]      test -> test

 ## Going back to the dev branch and delete the test branch
 
PS C:\Users\DONDOU\Desktop\Git_Exercise> git checkout  dev
Switched to branch 'dev'
PS C:\Users\DONDOU\Desktop\Git_Exercise> git branch -D test
Deleted branch test (was 3d99a12).
PS C:\Users\DONDOU\Desktop\Git_Exercise> git push origin --delete test
To https://github.com/dondou21/Git-exercises.git
 - [deleted]         test
PS C:\Users\DONDOU\Desktop\Git_Exercise> 
```


# Bundle 2

# Exercise 1

``` bash

## Git initialization

PS C:\Users\DONDOU\Desktop\Git-exercises> git init 
Reinitialized existing Git repository in C:/Users/DONDOU/Desktop/Git-exercises/.git/
PS C:\Users\DONDOU\Desktop\Git-exercises> git status
On branch main
Your branch is up to date with 'origin/main'.
nothing to commit, working tree clean

## Creating the branch ft/bundle-2 & services.html page

PS C:\Users\DONDOU\Desktop\Git-exercises> git checkout -b ft/bundle-2
Switched to a new branch 'ft/bundle-2'
On branch ft/bundle-2
nothing to commit, working tree clean
On branch ft/bundle-2
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        services.html

nothing added to commit but untracked files present (use "git add" to track)

## Committing and pushing the changes 

PS C:\Users\DONDOU\Desktop\Git-exercises> git add services.html 
PS C:\Users\DONDOU\Desktop\Git-exercises> git commit -m 'Creation of services.html'
[ft/bundle-2 faa6553] Creation of services.html
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 services.html
PS C:\Users\DONDOU\Desktop\Git-exercises> git status
On branch ft/bundle-2
nothing to commit, working tree clean
PS C:\Users\DONDOU\Desktop\Git-exercises> git push 
fatal: The current branch ft/bundle-2 has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/bundle-2

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

## Creating for the pull request

PS C:\Users\DONDOU\Desktop\Git-exercises> git push --set-upstream origin ft/bundle-2
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 289 bytes | 3.00 KiB/s, done.
Total 3 (delta 0), reused 1 (delta 0), pack-reused 0 (from 0)
remote: 
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/dondou21/Git-exercises/pull/new/ft/bundle-2
remote:
To https://github.com/dondou21/Git-exercises.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2
branch 'ft/bundle-2' set up to track 'origin/ft/bundle-2'.
PS C:\Users\DONDOU\Desktop\Git-exercises> 

```