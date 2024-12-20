# Git Project

The exercises to get good level in Git

# Bunlde1 

## Exercice 1

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



## Exercise 2

``` bash

### Initialisation of git

gymkubahoii@Kubahos-iMac-2 Git-exercises % git init
Reinitialized existing Git repository in /Users/gymkubahoii/Documents/dondou/Git-exercises/.git/

### Creating new branch for the exercise

gymkubahoii@Kubahos-iMac-2 Git-exercises % git checkout -b exo2
Switched to a new branch 'exo2'
gymkubahoii@Kubahos-iMac-2 Git-exercises % git status
On branch exo2
nothing added to commit but untracked files present (use "git add" to track)

### creating of the home.html

gymkubahoii@Kubahos-iMac-2 Git-exercises % git status
On branch exo2
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        home.html

nothing added to commit but untracked files present (use "git add" to track)

### Stash and save the current changes

gymkubahoii@Kubahos-iMac-2 Git-exercises % git stash list
gymkubahoii@Kubahos-iMac-2 Git-exercises % git add home.html
gymkubahoii@Kubahos-iMac-2 Git-exercises % git status    
On branch exo2
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   home.html

gymkubahoii@Kubahos-iMac-2 Git-exercises % git stash list   
gymkubahoii@Kubahos-iMac-2 Git-exercises % git stash 
Saved working directory and index state WIP on exo2: 1e7fa7a Merge pull request #1 from dondou21/dev
gymkubahoii@Kubahos-iMac-2 Git-exercises % git stash list
stash@{0}: WIP on exo2: 1e7fa7a Merge pull request #1 from dondou21/dev

### Creation of about.html and stash save

gymkubahoii@Kubahos-iMac-2 Git-exercises % git add .    
gymkubahoii@Kubahos-iMac-2 Git-exercises % git stash 
Saved working directory and index state WIP on exo2: 1e7fa7a Merge pull request #1 from dondou21/dev
gymkubahoii@Kubahos-iMac-2 Git-exercises % git status 
On branch exo2
nothing to commit, working tree clean
gymkubahoii@Kubahos-iMac-2 Git-exercises % git stash list 
stash@{0}: WIP on exo2: 1e7fa7a Merge pull request #1 from dondou21/dev
stash@{1}: WIP on exo2: 1e7fa7a Merge pull request #1 from dondou21/dev

### Creation of team.html and stash save

gymkubahoii@Kubahos-iMac-2 Git-exercises % git status 
On branch exo2
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        team.html

nothing added to commit but untracked files present (use "git add" to track)
gymkubahoii@Kubahos-iMac-2 Git-exercises % git add team.html
gymkubahoii@Kubahos-iMac-2 Git-exercises % git stash 
Saved working directory and index state WIP on exo2: 1e7fa7a Merge pull request #1 from dondou21/dev

### Check the current status

gymkubahoii@Kubahos-iMac-2 Git-exercises % git stash list 
stash@{0}: WIP on exo2: 1e7fa7a Merge pull request #1 from dondou21/dev
stash@{1}: WIP on exo2: 1e7fa7a Merge pull request #1 from dondou21/dev
stash@{2}: WIP on exo2: 1e7fa7a Merge pull request #1 from dondou21/dev

### Stash pop to restore th echanges of the about.html page

gymkubahoii@Kubahos-iMac-2 Git-exercises %  git stash pop stash@{1}
On branch exo2
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

Dropped stash@{1} (e1c3d9cf7c10d40f6ef49e7a781808e57afb192c)

### Checking for the current status

gymkubahoii@Kubahos-iMac-2 Git-exercises % git stash list 
stash@{0}: WIP on exo2: 1e7fa7a Merge pull request #1 from dondou21/dev
stash@{1}: WIP on exo2: 1e7fa7a Merge pull request #1 from dondou21/dev

### Stash pop to bring back the home.html pages changes

gymkubahoii@Kubahos-iMac-2 Git-exercises % git stash  pop stash@{1} 
Auto-merging home.html
CONFLICT (add/add): Merge conflict in home.html
On branch exo2
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Unmerged paths:
  (use "git restore --staged <file>..." to unstage)
  (use "git add <file>..." to mark resolution)
        both added:      home.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

The stash entry is kept in case you need it again.

### Commit and push current changes

gymkubahoii@Kubahos-iMac-2 Git-exercises % git add --all
gymkubahoii@Kubahos-iMac-2 Git-exercises % git status
On branch exo2
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   README.md
        new file:   about.html
        new file:   home.html

gymkubahoii@Kubahos-iMac-2 Git-exercises % git commit -m 'setup the home and about page with little modification on the README.md file'
[exo2 ca7aaf0] setup the home and about page with little modification on the README.md file
 3 files changed, 15 insertions(+), 1 deletion(-)
 create mode 100644 about.html
 create mode 100644 home.html
gymkubahoii@Kubahos-iMac-2 Git-exercises % git push 
fatal: The current branch exo2 has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin exo2

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

gymkubahoii@Kubahos-iMac-2 Git-exercises % git push --set-upstream origin exo2
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (5/5), 591 bytes | 591.00 KiB/s, done.
Total 5 (delta 1), reused 1 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'exo2' on GitHub by visiting:
remote:      https://github.com/dondou21/Git-exercises/pull/new/exo2
remote: 
To https://github.com/dondou21/Git-exercises.git
 * [new branch]      exo2 -> exo2
branch 'exo2' set up to track 'origin/exo2'.
gymkubahoii@Kubahos-iMac-2 Git-exercises % git status 
On branch exo2
Your branch is up to date with 'origin/exo2'.

nothing to commit, working tree clean
gymkubahoii@Kubahos-iMac-2 Git-exercises % git stash list 
stash@{0}: WIP on exo2: 1e7fa7a Merge pull request #1 from dondou21/dev
stash@{1}: WIP on exo2: 1e7fa7a Merge pull request #1 from dondou21/dev
gymkubahoii@Kubahos-iMac-2 Git-exercises % git stash
No local changes to save

### Stash pop to restore the changes of the team.html page index

gymkubahoii@Kubahos-iMac-2 Git-exercises % git stash pop
On branch exo2
Your branch is up to date with 'origin/exo2'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Dropped refs/stash@{0} (eb614946388582a54a3fcf22c95d539e56a27950)

### Reset the current changes using git rest and go back to the changes without  the team.html page

gymkubahoii@Kubahos-iMac-2 Git-exercises % git reset --hard
HEAD is now at ca7aaf0 setup the home and about page with little modification on the README.md file
gymkubahoii@Kubahos-iMac-2 Git-exercises % git status
On branch exo2
Your branch is up to date with 'origin/exo2'.

nothing to commit, working tree clean
gymkubahoii@Kubahos-iMac-2 Git-exercises % 

```