This is the README.md file.
# Bundle 1
## Exercise 1
```
HP@Hassan MINGW64 ~
$ mkdir gym-GIT-exercises

HP@Hassan MINGW64 ~
$ cd gym-GIT-exercises/

HP@Hassan MINGW64 ~/gym-GIT-exercises
$ git init
Initialized empty Git repository in C:/Users/HP/gym-GIT-exercises/.git/

HP@Hassan MINGW64 ~/gym-GIT-exercises (main)
$ touch README.md

HP@Hassan MINGW64 ~/gym-GIT-exercises (main)
$ vi README.md

HP@Hassan MINGW64 ~/gym-GIT-exercises (main)
$ mv main master
mv: cannot stat 'main': No such file or directory

HP@Hassan MINGW64 ~/gym-GIT-exercises (main)
$ git branch -M master

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git add .
warning: in the working copy of 'README.md', LF will be replaced by CRLF the next time Git touches it

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ ls
README.md


HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   README.md


HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git commit -m 'first commit'
[master (root-commit) 08a565e] first commit
 1 file changed, 1 insertion(+)
 create mode 100644 README.md

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git push
fatal: No configured push destination.
Either specify the URL from the command-line or configure a remote repository using

    git remote add <name> <url>

and then push using the remote name

    git push <name>


HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ ^C

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git remote add origin https://github.com/Hassanadelani1/gym-GIT-exercises.git

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git push -u origin master
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 240 bytes | 80.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/Hassanadelani1/gym-GIT-exercises.git
 * [new branch]      master -> master
branch 'master' set up to track 'origin/master'.

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$
HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git checkout dev
Switched to branch 'dev'

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git checkout dev
Already on 'dev'

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git checkout test
error: pathspec 'test' did not match any file(s) known to git

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git branch test

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git checkout test
Switched to branch 'test'

HP@Hassan MINGW64 ~/gym-GIT-exercises (test)
$ git checkout dev
Switched to branch 'dev'

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git branch -d test
Deleted branch test (was a7d2f3c).

```
# Bundle 1
## Excercise 2
```
HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git checkout dev
Switched to branch 'dev'

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git checkout master
Switched to branch 'master'
Your branch is up to date with 'origin/master'.

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ ls
README.md

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git checkout dev
Switched to branch 'dev'

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ ls
README.md

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ vi home.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ ls
README.md  home.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ code home.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ vi home.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git status
On branch dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        home.html

nothing added to commit but untracked files present (use "git add" to track)

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git stash home.html
fatal: subcommand wasn't specified; 'push' can't be assumed due to unexpected token 'home.html'

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git stash
No local changes to save

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git add .

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git status
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   home.html


HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git stash home.html
fatal: subcommand wasn't specified; 'push' can't be assumed due to unexpected token 'home.html'

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git stash
Saved working directory and index state WIP on dev: be604d4 Update README.md

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git chekout master
git: 'chekout' is not a git command. See 'git --help'.

The most similar command is
        checkout

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git checkout master
Switched to branch 'master'
Your branch is up to date with 'origin/master'.

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git checkout dev
Switched to branch 'dev'

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ touch about.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ code about.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ ls
README.md  about.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$


HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git stash -u
Saved working directory and index state WIP on dev: be604d4 Update README.md

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ ls
README.md

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ touch team.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ code team.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ ls
README.md  team.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git add .

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git stash
Saved working directory and index state WIP on dev: be604d4 Update README.md

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ ls
README.md

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git stash list
stash@{0}: WIP on dev: be604d4 Update README.md
stash@{1}: WIP on dev: be604d4 Update README.md
stash@{2}: WIP on dev: be604d4 Update README.md
stash@{3}: WIP on master: be604d4 Update README.md
stash@{4}: WIP on master: be604d4 Update README.md
stash@{5}: WIP on master: be604d4 Update README.md
stash@{6}: WIP on master: be604d4 Update README.md

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git stash pop about.html
error: about.html is not a valid reference

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git pop be604d4
git: 'pop' is not a git command. See 'git --help'.

The most similar command is
        log

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git stash pop be604d4
fatal: 'be604d4' is not a stash-like commit

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git stash list
stash@{0}: WIP on dev: be604d4 Update README.md
stash@{1}: WIP on dev: be604d4 Update README.md
stash@{2}: WIP on dev: be604d4 Update README.md
stash@{3}: WIP on master: be604d4 Update README.md
stash@{4}: WIP on master: be604d4 Update README.md
stash@{5}: WIP on master: be604d4 Update README.md
stash@{6}: WIP on master: be604d4 Update README.md

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git stash pop
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Dropped refs/stash@{0} (13aa38a4d1e60d3a38b2c8f99e8f990471c7e68b)

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git stash pop stash@{0}
Already up to date.
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        about.html

Dropped stash@{0} (237bb1482a904b4fdda8f5e3363fa91d5a10a9d4)

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git status
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        about.html


HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git add .

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git status
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   team.html


HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git stash list
stash@{0}: WIP on dev: be604d4 Update README.md
stash@{1}: WIP on master: be604d4 Update README.md
stash@{2}: WIP on master: be604d4 Update README.md
stash@{3}: WIP on master: be604d4 Update README.md
stash@{4}: WIP on master: be604d4 Update README.md

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git stash pop stash@{0}
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html
        new file:   team.html

Dropped stash@{0} (f99585cfcc2117a1ce3ad7d946378db60add65a9)

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git stash pop stash@{4}
fatal: log for 'stash' only has 4 entries

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git stash list
stash@{0}: WIP on master: be604d4 Update README.md
stash@{1}: WIP on master: be604d4 Update README.md
stash@{2}: WIP on master: be604d4 Update README.md
stash@{3}: WIP on master: be604d4 Update README.md

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git stash pop stash@{0}
Already up to date.
team.html already exists, no checkout
error: could not restore untracked files from stash
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html
        new file:   team.html

The stash entry is kept in case you need it again.

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git stash list
stash@{0}: WIP on master: be604d4 Update README.md
stash@{1}: WIP on master: be604d4 Update README.md
stash@{2}: WIP on master: be604d4 Update README.md
stash@{3}: WIP on master: be604d4 Update README.md

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git stash pop stash@{3}
Auto-merging home.html
CONFLICT (add/add): Merge conflict in home.html
Auto-merging team.html
CONFLICT (add/add): Merge conflict in team.html
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Unmerged paths:
  (use "git restore --staged <file>..." to unstage)
  (use "git add <file>..." to mark resolution)
        both added:      home.html
        both added:      team.html

The stash entry is kept in case you need it again.

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git status
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Unmerged paths:
  (use "git restore --staged <file>..." to unstage)
  (use "git add <file>..." to mark resolution)
        both added:      home.html
        both added:      team.html


HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git stash list
stash@{0}: WIP on master: be604d4 Update README.md
stash@{1}: WIP on master: be604d4 Update README.md
stash@{2}: WIP on master: be604d4 Update README.md
stash@{3}: WIP on master: be604d4 Update README.md

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git stash pop stash@{3}
home.html: needs merge
team.html: needs merge
error: could not write index
The stash entry is kept in case you need it again.

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git stash pop stash@{3}
home.html: needs merge
team.html: needs merge
error: could not write index
The stash entry is kept in case you need it again.

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git stash pop stash@{2}
home.html: needs merge
team.html: needs merge
error: could not write index
The stash entry is kept in case you need it again.

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git stash pop stash@{1}
home.html: needs merge
team.html: needs merge
error: could not write index
The stash entry is kept in case you need it again.

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git stash list
stash@{0}: WIP on master: be604d4 Update README.md
stash@{1}: WIP on master: be604d4 Update README.md
stash@{2}: WIP on master: be604d4 Update README.md
stash@{3}: WIP on master: be604d4 Update README.md

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git stash pop stash@{0}
home.html: needs merge
team.html: needs merge
error: could not write index
The stash entry is kept in case you need it again.

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git stash list
stash@{0}: WIP on master: be604d4 Update README.md
stash@{1}: WIP on master: be604d4 Update README.md
stash@{2}: WIP on master: be604d4 Update README.md
stash@{3}: WIP on master: be604d4 Update README.md

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git stash pop stash@{3}
home.html: needs merge
team.html: needs merge
error: could not write index
The stash entry is kept in case you need it again.

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git stash list
stash@{0}: WIP on master: be604d4 Update README.md
stash@{1}: WIP on master: be604d4 Update README.md
stash@{2}: WIP on master: be604d4 Update README.md
stash@{3}: WIP on master: be604d4 Update README.md

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git status
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Unmerged paths:
  (use "git restore --staged <file>..." to unstage)
  (use "git add <file>..." to mark resolution)
        both added:      home.html
        both added:      team.html


HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ rm home.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ rm team.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ ls
README.md  about.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git stash list
stash@{0}: WIP on master: be604d4 Update README.md
stash@{1}: WIP on master: be604d4 Update README.md
stash@{2}: WIP on master: be604d4 Update README.md
stash@{3}: WIP on master: be604d4 Update README.md

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git stash pop stash@{3}
home.html: needs merge
team.html: needs merge
error: could not write index
The stash entry is kept in case you need it again.

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git stash list
stash@{0}: WIP on master: be604d4 Update README.md
stash@{1}: WIP on master: be604d4 Update README.md
stash@{2}: WIP on master: be604d4 Update README.md
stash@{3}: WIP on master: be604d4 Update README.md

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git stash pop stash@{0}
home.html: needs merge
team.html: needs merge
error: could not write index
The stash entry is kept in case you need it again.

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git stash list
stash@{0}: WIP on master: be604d4 Update README.md
stash@{1}: WIP on master: be604d4 Update README.md
stash@{2}: WIP on master: be604d4 Update README.md
stash@{3}: WIP on master: be604d4 Update README.md

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git stash list
stash@{0}: WIP on master: be604d4 Update README.md
stash@{1}: WIP on master: be604d4 Update README.md
stash@{2}: WIP on master: be604d4 Update README.md
stash@{3}: WIP on master: be604d4 Update README.md

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git stash pop stash@{0}
home.html: needs merge
team.html: needs merge
error: could not write index
The stash entry is kept in case you need it again.

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git stash pop stash@{2}
home.html: needs merge
team.html: needs merge
error: could not write index
The stash entry is kept in case you need it again.

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git stash list
stash@{0}: WIP on master: be604d4 Update README.md
stash@{1}: WIP on master: be604d4 Update README.md
stash@{2}: WIP on master: be604d4 Update README.md
stash@{3}: WIP on master: be604d4 Update README.md

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git checkout master
home.html: needs merge
team.html: needs merge
error: you need to resolve your current index first

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git restore
fatal: you must specify path(s) to restore

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ ls
README.md  about.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ ls
README.md  about.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ rm home.html
rm: cannot remove 'home.html': No such file or directory

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git restore home.html
error: path 'home.html' is unmerged

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git checkout master
home.html: needs merge
team.html: needs merge
error: you need to resolve your current index first

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git add .

HP@Hassan MINGW64 ~/gym-GIT-exercises (dev)
$ git checkout master
A       about.html
Switched to branch 'master'
Your branch is up to date with 'origin/master'.

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ ls
README.md  about.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git stash list
stash@{0}: WIP on master: be604d4 Update README.md
stash@{1}: WIP on master: be604d4 Update README.md
stash@{2}: WIP on master: be604d4 Update README.md
stash@{3}: WIP on master: be604d4 Update README.md

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ rm about.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ ls
README.md

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git stash pop stash@{0}
Already up to date.
On branch master
Your branch is up to date with 'origin/master'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        deleted:    about.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        team.html

Dropped stash@{0} (b1697c9e4f06e7c94f5f4240c4a15b1b87128509)

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git stash list
stash@{0}: WIP on master: be604d4 Update README.md
stash@{1}: WIP on master: be604d4 Update README.md
stash@{2}: WIP on master: be604d4 Update README.md

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ ls
README.md  team.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git stash pop stash@{0}
Already up to date.
On branch master
Your branch is up to date with 'origin/master'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        deleted:    about.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        home.html
        team.html

Dropped stash@{0} (410933c35ce41ec46abdd8cbde0946424e5dd090)

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git stash pop stash@{1}
error: The following untracked working tree files would be overwritten by merge:
        home.html
        team.html
Please move or remove them before you merge.
Aborting
On branch master
Your branch is up to date with 'origin/master'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        deleted:    about.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        home.html
        team.html

The stash entry is kept in case you need it again.

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git stash list
stash@{0}: WIP on master: be604d4 Update README.md
stash@{1}: WIP on master: be604d4 Update README.md

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git stash pop stash@{1}
error: The following untracked working tree files would be overwritten by merge:
        home.html
        team.html
Please move or remove them before you merge.
Aborting
On branch master
Your branch is up to date with 'origin/master'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        deleted:    about.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        home.html
        team.html

The stash entry is kept in case you need it again.

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git stash list
stash@{0}: WIP on master: be604d4 Update README.md
stash@{1}: WIP on master: be604d4 Update README.md

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git stash pop stash@{0}
error: The following untracked working tree files would be overwritten by merge:
        home.html
Please move or remove them before you merge.
Aborting
On branch master
Your branch is up to date with 'origin/master'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        deleted:    about.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        home.html
        team.html

The stash entry is kept in case you need it again.

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git stash list
stash@{0}: WIP on master: be604d4 Update README.md
stash@{1}: WIP on master: be604d4 Update README.md

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ ls
README.md  home.html  team.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git add .

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git stash list
stash@{0}: WIP on master: be604d4 Update README.md
stash@{1}: WIP on master: be604d4 Update README.md

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git stash pop stash@{0}
Auto-merging home.html
CONFLICT (add/add): Merge conflict in home.html
On branch master
Your branch is up to date with 'origin/master'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Unmerged paths:
  (use "git restore --staged <file>..." to unstage)
  (use "git add <file>..." to mark resolution)
        both added:      home.html

The stash entry is kept in case you need it again.

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git stash list
stash@{0}: WIP on master: be604d4 Update README.md
stash@{1}: WIP on master: be604d4 Update README.md

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git stash pop stash@{1}
home.html: needs merge
error: could not write index
The stash entry is kept in case you need it again.

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git stash list
stash@{0}: WIP on master: be604d4 Update README.md
stash@{1}: WIP on master: be604d4 Update README.md

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ ls
README.md  home.html  team.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ rm home.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git stash list
stash@{0}: WIP on master: be604d4 Update README.md
stash@{1}: WIP on master: be604d4 Update README.md

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git stash pop stash@{1}
home.html: needs merge
error: could not write index
The stash entry is kept in case you need it again.

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git add .

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ ls
README.md  team.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git stash pop stash@{1}
Auto-merging team.html
CONFLICT (add/add): Merge conflict in team.html
On branch master
Your branch is up to date with 'origin/master'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   home.html

Unmerged paths:
  (use "git restore --staged <file>..." to unstage)
  (use "git add <file>..." to mark resolution)
        both added:      team.html

The stash entry is kept in case you need it again.

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git stash list
stash@{0}: WIP on master: be604d4 Update README.md
stash@{1}: WIP on master: be604d4 Update README.md

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git stash pop stash@{1}
team.html: needs merge
error: could not write index
The stash entry is kept in case you need it again.

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git add .

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ ls
README.md  home.html  team.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git stash pop stash@{0}
Auto-merging home.html
CONFLICT (add/add): Merge conflict in home.html
On branch master
Your branch is up to date with 'origin/master'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Unmerged paths:
  (use "git restore --staged <file>..." to unstage)
  (use "git add <file>..." to mark resolution)
        both added:      home.html

The stash entry is kept in case you need it again.

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ ls
README.md  home.html  team.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git add .

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ ls
README.md  home.html  team.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ ls
README.md  home.html  team.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git stash pop stash@{0}
Auto-merging home.html
CONFLICT (add/add): Merge conflict in home.html
On branch master
Your branch is up to date with 'origin/master'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Unmerged paths:
  (use "git restore --staged <file>..." to unstage)
  (use "git add <file>..." to mark resolution)
        both added:      home.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   team.html

The stash entry is kept in case you need it again.

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git stash list
stash@{0}: WIP on master: be604d4 Update README.md
stash@{1}: WIP on master: be604d4 Update README.md

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ ls'
>
> ^C
s
HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ ls
README.md  home.html  team.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ touch about.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ code about.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git status
On branch master
Your branch is up to date with 'origin/master'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Unmerged paths:
  (use "git restore --staged <file>..." to unstage)
  (use "git add <file>..." to mark resolution)
        both added:      home.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   team.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        about.html


HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git add .

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git commit -m "commiting the changes"
[master 148ffde] commiting the changes
 3 files changed, 48 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html
 create mode 100644 team.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git push
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 4 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (5/5), 820 bytes | 273.00 KiB/s, done.
Total 5 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/Hassanadelani1/gym-GIT-exercises.git
   be604d4..148ffde  master -> master

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git stash list
stash@{0}: WIP on master: be604d4 Update README.md
stash@{1}: WIP on master: be604d4 Update README.md

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git stash list
stash@{0}: WIP on master: be604d4 Update README.md
stash@{1}: WIP on master: be604d4 Update README.md

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git reset --hard
HEAD is now at 148ffde commiting the changes

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ ls
README.md  about.html  home.html  team.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$
```
# Bundle 2
## Excercise 2
HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/service-redesign)
$ ls
README.md  about.html  home.html  team.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/service-redesign)
$ l
bash: l: command not found
s
HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/service-redesign)
$ ls
README.md  about.html  home.html  team.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/service-redesign)
$ git checkout master
Switched to branch 'master'
Your branch is up to date with 'origin/master'.

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ ls
README.md  about.html  home.html  team.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git pull
remote: Enumerating objects: 9, done.
remote: Counting objects: 100% (8/8), done.
remote: Compressing objects: 100% (5/5), done.
remote: Total 5 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (5/5), 4.47 KiB | 101.00 KiB/s, done.
From https://github.com/Hassanadelani1/gym-GIT-exercises
   148ffde..3d95f2e  master     -> origin/master
Updating 148ffde..3d95f2e
Fast-forward
 README.md     | 923 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++-
 services.html |  11 +
 2 files changed, 932 insertions(+), 2 deletions(-)
 create mode 100644 services.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ ls
README.md  about.html  home.html  services.html  team.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ ls
README.md  about.html  home.html  services.html  team.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git branch
  dev
  ft/bundle-2
  ft/service-redesign
* master

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git checkout ft/service-redesigned
error: pathspec 'ft/service-redesigned' did not match any file(s) known to git

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/service-redesign)
$ ls
README.md  about.html  home.html  team.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/service-redesign)
$ git branch master
fatal: a branch named 'master' already exists

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/service-redesign)
$ git checkout master
Switched to branch 'master'
Your branch is up to date with 'origin/master'.

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git branch -D ft/service-redesign
Deleted branch ft/service-redesign (was 148ffde).

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git branch ft/service-redesign

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/service-redesign)
$ ls
README.md  about.html  home.html  services.html  team.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/service-redesign)
$ code services.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/service-redesign)
$ git add .

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/service-redesign)
$ git commit -m 'made some changes to the services page'
[ft/service-redesign a4f0cb3] made some changes to the services page
 1 file changed, 1 insertion(+)

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/service-redesign)
$ git push
fatal: The current branch ft/service-redesign has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/service-redesign

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/service-redesign)
$  git push --set-upstream origin ft/service-redesign
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 344 bytes | 172.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/Hassanadelani1/gym-GIT-exercises/pull/new/ft/service-redesign
remote:
To https://github.com/Hassanadelani1/gym-GIT-exercises.git
 * [new branch]      ft/service-redesign -> ft/service-redesign
branch 'ft/service-redesign' set up to track 'origin/ft/service-redesign'.

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/service-redesign)
$ git branch master
fatal: a branch named 'master' already exists

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/service-redesign)
$ git checkout master
Switched to branch 'master'
Your branch is up to date with 'origin/master'.

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ ls
README.md  about.html  home.html  services.html  team.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ code services.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git pull
remote: Enumerating objects: 1, done.
remote: Counting objects: 100% (1/1), done.
remote: Total 1 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (1/1), 922 bytes | 102.00 KiB/s, done.
From https://github.com/Hassanadelani1/gym-GIT-exercises
   3d95f2e..64a2e42  master     -> origin/master
Updating 3d95f2e..64a2e42
Fast-forward
 services.html | 1 +
 1 file changed, 1 insertion(+)

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ code services.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ ls
README.md  about.html  home.html  services.html  team.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git add .
g
HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git commit -m 'made some changes to the services file'
[master c5e7838] made some changes to the services file
 1 file changed, 1 insertion(+), 1 deletion(-)

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 342 bytes | 171.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/Hassanadelani1/gym-GIT-exercises.git
   64a2e42..c5e7838  master -> master

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'
Your branch is up to date with 'origin/ft/service-redesign'.

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/service-redesign)
$ git diff master ft/service-redesign
diff --git a/services.html b/services.html
index d1d5676..d103b92 100644
--- a/services.html
+++ b/services.html
@@ -7,6 +7,6 @@
 </head>
 <body>
     <h2>Services page</h2>
-    <p>The changes made(from the master branch)</p>
+    <p>The changes made</p>
 </body>
 </html>
\ No newline at end of file

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/service-redesign)
$ git switch main
fatal: invalid reference: main

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/service-redesign)
$ git switch master
Switched to branch 'master'
Your branch is up to date with 'origin/master'.

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git merge ft/service-redesign
Already up to date.

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git pull
Already up to date.

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git merge
Already up to date.

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git switch ft/service-redesign
Switched to branch 'ft/service-redesign'
Your branch is up to date with 'origin/ft/service-redesign'.

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/service-redesign)
$ git pull
Already up to date.

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/service-redesign)
$ git diff master ft/service-redesign
diff --git a/services.html b/services.html
index d1d5676..d103b92 100644
--- a/services.html
+++ b/services.html
@@ -7,6 +7,6 @@
 </head>
 <body>
     <h2>Services page</h2>
-    <p>The changes made(from the master branch)</p>
+    <p>The changes made</p>
 </body>
 </html>
\ No newline at end of file

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/service-redesign)
$ gitpull
bash: gitpull: command not found

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/service-redesign)
$ git pull
Already up to date.

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/service-redesign)
$ git switch master
Switched to branch 'master'
Your branch is up to date with 'origin/master'.

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git pull
Already up to date.

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git merge ft/service-redesign
Already up to date.

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git status
On branch master
Your branch is up to date with 'origin/master'.

nothing to commit, working tree clean

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$

