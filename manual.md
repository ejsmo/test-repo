## git manual. Walkthrough

##cloning a repo from the Gitub
P@PELAP ~
$ git clone https://github.com/vannorden/test-repo.git
Cloning into 'test-repo'...
remote: Counting objects: 3, done.
remote: Total 3 (delta 0), reused 0 (delta 0)
Unpacking objects: 100% (3/3), done.
Checking connectivity... done.


##setting the working directory
P@PELAP ~
$ cd test-repo


##checking the content of the working directory
P@PELAP ~/test-repo (master)
$ ls
README.md

## checking existing connections
P@PELAP ~/test-repo (master)
$ git remote -v
origin  https://github.com/vannorden/test-repo.git (fetch)
origin  https://github.com/vannorden/test-repo.git (push)


##creating a new file
P@PELAP ~/test-repo (master)
$ touch new.md


##checking the status
P@PELAP ~/test-repo (master)
$ git status
On branch master
Your branch is up-to-date with 'origin/master'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   README.md

Untracked files:
  (use "git add <file>..." to include in what will be committed)

        new.md

no changes added to commit (use "git add" and/or "git commit -a")


## adding modification to all files
P@PELAP ~/test-repo (master)
$ git add .

