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


## adding modification to all files (intermediate level, not yet ##uploaded)
P@PELAP ~/test-repo (master)
$ git add .


## another intermediate level, still not yey uploaded
P@PELAP ~/test-repo (master)
$ git commit -m "Testing"
[master 99c141c] Testing
 3 files changed, 70 insertions(+), 1 deletion(-)
 create mode 100644 manual.md
 create mode 100644 new.md


## getting log of changes
P@PELAP ~/test-repo (master)
$ git log
commit 99c141c2a2bc199fcd790040f9b27124a602c821
Author: P <piotr.akanowicz@gmail.com>
Date:   Sat Jul 19 19:35:48 2014 +0200

    Testing

commit 5a236b8e275f019e7253e15070f5a68b122716d1
Author: vannorden <piotr.akanowicz@gmail.com>
Date:   Sat Jul 19 19:12:24 2014 +0200

    Initial commit


## pushing/uploading changes
P@PELAP ~/test-repo (master)
$ git push origin master
Username for 'https://github.com': vannorden
Password for 'https://vannorden@github.com':
Counting objects: 7, done.
Compressing objects: 100% (5/5), done.
Writing objects: 100% (5/5), 1015 bytes | 0 bytes/s, done.
Total 5 (delta 0), reused 0 (delta 0)
To https://github.com/vannorden/test-repo.git
   5a236b8..99c141c  master -> master

##
[LINK TO A WRITTEN TUTORIAL](http://www.dataschool.io/git-quick-reference-for-beginners)
[LINK TO A TUTORIAL ON YT](https://www.youtube.com/playlist?list=PL5-da3qGB5IBLMp7LtN8Nc3Efd4hJq0kD)

##this is secondary heading
### this is tertiary heading

* bullet1
* bullet2 etc.