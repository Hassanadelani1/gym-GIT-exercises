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
# Bundle 3
## Excercise 1
```
HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/contact-page)
$ git log
commit c5e7838e72f9106200fb5da5ac63f5f5e32d1c6a (HEAD -> ft/contact-page, origin/master, master)
commit c5e7838e72f9106200fb5da5ac63f5f5e32d1c6a (HEAD -> ft/contact-page, origin/master, master)
Author: Hassanadelani1 <luqmanadelani1@gmail.com>
Date:   Wed Dec 18 13:37:55 2024 +0200

    made some changes to the services file

commit 64a2e4216b4ca4e5f3d88936cece51ab6958da8b
Merge: 3d95f2e a4f0cb3
Author: Hassan Adelani Luqman <luqmanadelani1@gmail.com>
Date:   Wed Dec 18 13:33:26 2024 +0200

    Merge pull request #2 from Hassanadelani1/ft/service-redesign

    made some changes to the services page

commit a4f0cb3bcea9916f3e95a2c40eda70a467b3d75e (origin/ft/service-redesign, ft/service-redesign)
Author: Hassanadelani1 <luqmanadelani1@gmail.com>
Date:   Wed Dec 18 13:30:37 2024 +0200

    made some changes to the services page

commit 3d95f2e176b71b9c96d6eccdc696003133da07ef
Merge: be9edb4 0c02a1e
Author: Hassan Adelani Luqman <luqmanadelani1@gmail.com>
Date:   Wed Dec 18 13:22:26 2024 +0200

    Merge pull request #1 from Hassanadelani1/ft/bundle-2

    bundle 2 exercise 1 (confirmed the pull request)

commit c5e7838e72f9106200fb5da5ac63f5f5e32d1c6a (HEAD -> ft/contact-page, origin/master, master)
Author: Hassanadelani1 <luqmanadelani1@gmail.com>
Date:   Wed Dec 18 13:37:55 2024 +0200

    made some changes to the services file

commit 64a2e4216b4ca4e5f3d88936cece51ab6958da8b
Merge: 3d95f2e a4f0cb3
Author: Hassan Adelani Luqman <luqmanadelani1@gmail.com>
Date:   Wed Dec 18 13:33:26 2024 +0200

    Merge pull request #2 from Hassanadelani1/ft/service-redesign

    made some changes to the services page

commit a4f0cb3bcea9916f3e95a2c40eda70a467b3d75e (origin/ft/service-redesign, ft/service-redesign)
Author: Hassanadelani1 <luqmanadelani1@gmail.com>
Date:   Wed Dec 18 13:30:37 2024 +0200

    made some changes to the services page

commit 3d95f2e176b71b9c96d6eccdc696003133da07ef
Merge: be9edb4 0c02a1e
Author: Hassan Adelani Luqman <luqmanadelani1@gmail.com>
Date:   Wed Dec 18 13:22:26 2024 +0200

    Merge pull request #1 from Hassanadelani1/ft/bundle-2

    bundle 2 exercise 1 (confirmed the pull request)

commit 0c02a1e31feea583faaca82340ea8a6f3d671d96 (origin/ft/bundle-2, ft/bundle-2)
Author: Hassanadelani1 <luqmanadelani1@gmail.com>
Date:   Wed Dec 18 12:04:25 2024 +0200

    bundle 2 exercise 1

commit be9edb41497d0e2a68c331569ca0624492c29e19
Author: Hassan Adelani Luqman <luqmanadelani1@gmail.com>
Date:   Wed Dec 18 11:29:55 2024 +0200

    Update README.md

commit 148ffdecc220040040111cd3820bf090e3fefe94
Author: Hassanadelani1 <luqmanadelani1@gmail.com>
Date:   Wed Dec 18 10:56:40 2024 +0200

    commiting the changes

commit be604d49942b898d5d708100f4416920189ca451 (dev)
Author: Hassan Adelani Luqman <luqmanadelani1@gmail.com>
Date:   Tue Dec 17 13:24:14 2024 +0200

    Update README.md

commit a7d2f3cc7d5cc8a7d695e813914a75ad1a53389a
Author: Hassan Adelani Luqman <luqmanadelani1@gmail.com>
Date:   Tue Dec 17 12:24:23 2024 +0200

    Update README.md

commit 08a565e86aaa3dfa9c80e579fa3fb0100153c6b9
Author: Hassanadelani1 <luqmanadelani1@gmail.com>
Date:   Tue Dec 17 12:20:00 2024 +0200

    first commit

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/contact-page)
$ git log --oneline]
fatal: unrecognized argument: --oneline]

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/contact-page)
$ git log --oneline
c5e7838 (HEAD -> ft/contact-page, origin/master, master) made some changes to the services file
64a2e42 Merge pull request #2 from Hassanadelani1/ft/service-redesign
a4f0cb3 (origin/ft/service-redesign, ft/service-redesign) made some changes to the services page
3d95f2e Merge pull request #1 from Hassanadelani1/ft/bundle-2
0c02a1e (origin/ft/bundle-2, ft/bundle-2) bundle 2 exercise 1
be9edb4 Update README.md
148ffde commiting the changes
be604d4 (dev) Update README.md
a7d2f3c Update README.md
08a565e first commit

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/contact-page)
$ git log ft/team-page
commit f23a2eb4068f7bc03933f413032e4192e6e857dc (origin/ft/team-page, ft/team-page)
Author: Hassanadelani1 <luqmanadelani1@gmail.com>
Date:   Wed Dec 18 13:56:43 2024 +0200

    made some changes to the team page

commit c5e7838e72f9106200fb5da5ac63f5f5e32d1c6a (HEAD -> ft/contact-page, origin/master, master)
Author: Hassanadelani1 <luqmanadelani1@gmail.com>
Date:   Wed Dec 18 13:37:55 2024 +0200

    made some changes to the services file

commit 64a2e4216b4ca4e5f3d88936cece51ab6958da8b
Merge: 3d95f2e a4f0cb3
Author: Hassan Adelani Luqman <luqmanadelani1@gmail.com>
Date:   Wed Dec 18 13:33:26 2024 +0200

    Merge pull request #2 from Hassanadelani1/ft/service-redesign

    made some changes to the services page

commit a4f0cb3bcea9916f3e95a2c40eda70a467b3d75e (origin/ft/service-redesign, ft/service-redesign)
Author: Hassanadelani1 <luqmanadelani1@gmail.com>
Date:   Wed Dec 18 13:30:37 2024 +0200

    made some changes to the services page

commit 3d95f2e176b71b9c96d6eccdc696003133da07ef
Merge: be9edb4 0c02a1e
Author: Hassan Adelani Luqman <luqmanadelani1@gmail.com>
Date:   Wed Dec 18 13:22:26 2024 +0200

    Merge pull request #1 from Hassanadelani1/ft/bundle-2

    bundle 2 exercise 1 (confirmed the pull request)

commit 0c02a1e31feea583faaca82340ea8a6f3d671d96 (origin/ft/bundle-2, ft/bundle-2)
Author: Hassanadelani1 <luqmanadelani1@gmail.com>
Date:   Wed Dec 18 12:04:25 2024 +0200

    bundle 2 exercise 1

commit f23a2eb4068f7bc03933f413032e4192e6e857dc (origin/ft/team-page, ft/team-page)
Author: Hassanadelani1 <luqmanadelani1@gmail.com>
Date:   Wed Dec 18 13:56:43 2024 +0200

    made some changes to the team page

commit c5e7838e72f9106200fb5da5ac63f5f5e32d1c6a (HEAD -> ft/contact-page, origin/master, master)
Author: Hassanadelani1 <luqmanadelani1@gmail.com>
Date:   Wed Dec 18 13:37:55 2024 +0200

    made some changes to the services file

commit 64a2e4216b4ca4e5f3d88936cece51ab6958da8b
Merge: 3d95f2e a4f0cb3
Author: Hassan Adelani Luqman <luqmanadelani1@gmail.com>
Date:   Wed Dec 18 13:33:26 2024 +0200

    Merge pull request #2 from Hassanadelani1/ft/service-redesign

    made some changes to the services page

commit a4f0cb3bcea9916f3e95a2c40eda70a467b3d75e (origin/ft/service-redesign, ft/service-redesign)
Author: Hassanadelani1 <luqmanadelani1@gmail.com>
Date:   Wed Dec 18 13:30:37 2024 +0200

    made some changes to the services page

commit 3d95f2e176b71b9c96d6eccdc696003133da07ef
Merge: be9edb4 0c02a1e
Author: Hassan Adelani Luqman <luqmanadelani1@gmail.com>
Date:   Wed Dec 18 13:22:26 2024 +0200

    Merge pull request #1 from Hassanadelani1/ft/bundle-2

    bundle 2 exercise 1 (confirmed the pull request)

commit 0c02a1e31feea583faaca82340ea8a6f3d671d96 (origin/ft/bundle-2, ft/bundle-2)
Author: Hassanadelani1 <luqmanadelani1@gmail.com>
Date:   Wed Dec 18 12:04:25 2024 +0200

    bundle 2 exercise 1

commit be9edb41497d0e2a68c331569ca0624492c29e19
Author: Hassan Adelani Luqman <luqmanadelani1@gmail.com>
Date:   Wed Dec 18 11:29:55 2024 +0200

    Update README.md

commit 148ffdecc220040040111cd3820bf090e3fefe94
Author: Hassanadelani1 <luqmanadelani1@gmail.com>
Date:   Wed Dec 18 10:56:40 2024 +0200

    commiting the changes

commit be604d49942b898d5d708100f4416920189ca451 (dev)
Author: Hassan Adelani Luqman <luqmanadelani1@gmail.com>
Date:   Tue Dec 17 13:24:14 2024 +0200

    Update README.md

commit a7d2f3cc7d5cc8a7d695e813914a75ad1a53389a
Author: Hassan Adelani Luqman <luqmanadelani1@gmail.com>
Date:   Tue Dec 17 12:24:23 2024 +0200

    Update README.md

commit 08a565e86aaa3dfa9c80e579fa3fb0100153c6b9
Author: Hassanadelani1 <luqmanadelani1@gmail.com>
Date:   Tue Dec 17 12:20:00 2024 +0200

    first commit


HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/contact-page)
$

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/contact-page)
$ git switch ft/team-page
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/team-page)
$ git rev-parse ft/team-page
f23a2eb4068f7bc03933f413032e4192e6e857dc

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/team-page)
$ git switch ft/contact-page
Switched to branch 'ft/contact-page'

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/contact-page)
$ git cherry-pick f23a2eb4068f7bc03933f413032e4192e6e857dc
[ft/contact-page 8a005cb] made some changes to the team page
 Date: Wed Dec 18 13:56:43 2024 +0200
 1 file changed, 1 insertion(+)

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/contact-page)
$ ls
README.md  about.html  home.html  service.html  services.html  team.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/contact-page)
$ git status
On branch ft/contact-page
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        service.html

nothing added to commit but untracked files present (use "git add" to track)

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/contact-page)
$ git add .

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/contact-page)
$ git commit -m 'made some changes to the contact page'
[ft/contact-page 8874f8f] made some changes to the contact page
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 service.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/contact-page)
$ git push
fatal: The current branch ft/contact-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/contact-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/contact-page)
$ git push --set-upstream origin ft/contact-page
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 4 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (6/6), 561 bytes | 93.00 KiB/s, done.
Total 6 (delta 3), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (3/3), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting:
remote:      https://github.com/Hassanadelani1/gym-GIT-exercises/pull/new/ft/contact-page
remote:
To https://github.com/Hassanadelani1/gym-GIT-exercises.git
 * [new branch]      ft/contact-page -> ft/contact-page
branch 'ft/contact-page' set up to track 'origin/ft/contact-page'.

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/contact-page)
$ git branch ft/faq-page

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/contact-page)
$ touch faq.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/contact-page)
$ code faq.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/contact-page)
$ git ststus
git: 'ststus' is not a git command. See 'git --help'.

The most similar command is
        status

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/contact-page)
$ git status
On branch ft/contact-page
Your branch is up to date with 'origin/ft/contact-page'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        faq.html

nothing added to commit but untracked files present (use "git add" to track)

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/contact-page)
$ git add .
gt
HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/contact-page)
$ git commit -m 'created the faq file'
[ft/contact-page e01e232] created the faq file
 1 file changed, 11 insertions(+)
 create mode 100644 faq.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/contact-page)
$ git push
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 432 bytes | 216.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/Hassanadelani1/gym-GIT-exercises.git
   8874f8f..e01e232  ft/contact-page -> ft/contact-page

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/contact-page)
$ git revert f23a2eb4068f7bc03933f413032e4192e6e857dc
[ft/contact-page 247a8be] Revert "made some changes to the team page"
 1 file changed, 1 deletion(-)

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/contact-page)
$ git status
On branch ft/contact-page
Your branch is ahead of 'origin/ft/contact-page' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/contact-page)
$ git add .

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/contact-page)
$ git status
On branch ft/contact-page
Your branch is ahead of 'origin/ft/contact-page' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/contact-page)
$ git commit -m 'reverted the changes in the last commit on the team page'
On branch ft/contact-page
Your branch is ahead of 'origin/ft/contact-page' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/contact-page)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 347 bytes | 347.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/Hassanadelani1/gym-GIT-exercises.git
   e01e232..247a8be  ft/contact-page -> ft/contact-page

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/contact-page)
$ git status
On branch ft/contact-page
Your branch is up to date with 'origin/ft/contact-page'.

nothing to commit, working tree clean
```
# Bundle 3
## Excersise 2
```
HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/home-page-redesign)
$ git checkout master
Switched to branch 'master'
Your branch is up to date with 'origin/master'.

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ ls
README.md  about.html  home.html  services.html  team.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ code about.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git status
On branch master
Your branch is up to date with 'origin/master'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   about.html

no changes added to commit (use "git add" and/or "git commit -a")

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git add .

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git commit -m 'made some changes to the about page'
[master 54f8d66] made some changes to the about page
 1 file changed, 1 insertion(+), 1 deletion(-)

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git push'
> ^C

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git push
To https://github.com/Hassanadelani1/gym-GIT-exercises.git
 ! [rejected]        master -> master (fetch first)
error: failed to push some refs to 'https://github.com/Hassanadelani1/gym-GIT-exercises.git'
hint: Updates were rejected because the remote contains work that you do not
hint: have locally. This is usually caused by another repository pushing to
hint: the same ref. If you want to integrate the remote changes, use
hint: 'git pull' before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git pull
remote: Enumerating objects: 12, done.
remote: Counting objects: 100% (11/11), done.
remote: Compressing objects: 100% (8/8), done.
remote: Total 8 (delta 5), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (8/8), 5.97 KiB | 82.00 KiB/s, done.
From https://github.com/Hassanadelani1/gym-GIT-exercises
   c5e7838..8f822e5  master     -> origin/master
Merge made by the 'ort' strategy.
 README.md | 696 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-
 team.html |   1 +
 2 files changed, 696 insertions(+), 1 deletion(-)

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git push
Enumerating objects: 9, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 4 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (5/5), 643 bytes | 214.00 KiB/s, done.
Total 5 (delta 3), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (3/3), completed with 3 local objects.
To https://github.com/Hassanadelani1/gym-GIT-exercises.git
   8f822e5..e9e6cbb  master -> master

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git switch ft/home-page-redesign
Switched to branch 'ft/home-page-redesign'

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/home-page-redesign)
$ git fetch origin

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/home-page-redesign)
$ git rebase main
fatal: invalid upstream 'main'

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/home-page-redesign)
$ git rebase master
warning: skipped previously applied commit 8a005cb
hint: use --reapply-cherry-picks to include skipped commits
hint: Disable this message with "git config advice.skippedCherryPicks false"
Successfully rebased and updated refs/heads/ft/home-page-redesign.

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/home-page-redesign)
$ ls
README.md  about.html  home.html  service.html  services.html  team.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/home-page-redesign)
$ code home.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/home-page-redesign)
$ git status
On branch ft/home-page-redesign
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   home.html

no changes added to commit (use "git add" and/or "git commit -a")

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/home-page-redesign)
$ git add .

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/home-page-redesign)
$ git push
fatal: The current branch ft/home-page-redesign has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/home-page-redesign

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/home-page-redesign)
$ git commit -m 'made changes to the home.html'
[ft/home-page-redesign 7449d44] made changes to the home.html
 1 file changed, 1 insertion(+)

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/home-page-redesign)
$ git push --set-upstream origin ft/home-page-redesign
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 4 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (6/6), 644 bytes | 161.00 KiB/s, done.
Total 6 (delta 3), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (3/3), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/home-page-redesign' on GitHub by visiting:
remote:      https://github.com/Hassanadelani1/gym-GIT-exercises/pull/new/ft/home-page-redesign
remote:
To https://github.com/Hassanadelani1/gym-GIT-exercises.git
 * [new branch]      ft/home-page-redesign -> ft/home-page-redesign
branch 'ft/home-page-redesign' set up to track 'origin/ft/home-page-redesign'.
```
# Bundle 4
## Exercise 1
```

HP@Hassan MINGW64 ~
$ ls
 -1.14-windows.xml
'3D Objects'/
 AppData/
'Application Data'@
 Contacts/
 Cookies@
 Documents/
 Downloads/
 IntelGraphicsProfiles/
'Local Settings'@
 MicrosoftEdgeBackups/
'My Documents'@
 NTUSER.DAT
 NTUSER.DAT{53b39e88-18c4-11ea-a811-000d3aa4692b}.TM.blf
 NTUSER.DAT{53b39e88-18c4-11ea-a811-000d3aa4692b}.TMContainer00000000000000000001.regtrans-ms
 NTUSER.DAT{53b39e88-18c4-11ea-a811-000d3aa4692b}.TMContainer00000000000000000002.regtrans-ms
 NetHood@
 OneDrive/
 PrintHood@
 PycharmProjects/
 Recent@
 SendTo@
'Start Menu'@
 Templates@
 Tracing/
 Videos/
'WPS Cloud Files'/
 a/
 anaconda3/
 c/
 gym-GIT-exercises/
 index.html
 index.js
 js
 letter.txt
 ntuser.dat.LOG1
 ntuser.dat.LOG2
 ntuser.ini
 prac
 vid.txt

HP@Hassan MINGW64 ~
$ cd gym-GIT-exercises/

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/home-page-redesign)
$ git checkout master
Switched to branch 'master'
Your branch is up to date with 'origin/master'.

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git remote add git-copy https://github.com/Hassanadelani1/git-copy

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git remote -v
git-copy        https://github.com/Hassanadelani1/git-copy (fetch)
git-copy        https://github.com/Hassanadelani1/git-copy (push)
origin  https://github.com/Hassanadelani1/gym-GIT-exercises.git (fetch)
origin  https://github.com/Hassanadelani1/gym-GIT-exercises.git (push)

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ ls
README.md  about.html  home.html  services.html  team.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ code home.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git status
On branch master
Your branch is up to date with 'origin/master'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   home.html

no changes added to commit (use "git add" and/or "git commit -a")

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git add .

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git commit -m 'made some changes to the home.html file'
[master 833812d] made some changes to the home.html file
 1 file changed, 1 insertion(+)

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git push origin master
To https://github.com/Hassanadelani1/gym-GIT-exercises.git
 ! [rejected]        master -> master (fetch first)
error: failed to push some refs to 'https://github.com/Hassanadelani1/gym-GIT-exercises.git'
hint: Updates were rejected because the remote contains work that you do not
hint: have locally. This is usually caused by another repository pushing to
hint: the same ref. If you want to integrate the remote changes, use
hint: 'git pull' before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git pull
remote: Enumerating objects: 5, done.
remote: Counting objects: 100% (5/5), done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (3/3), 2.02 KiB | 64.00 KiB/s, done.
From https://github.com/Hassanadelani1/gym-GIT-exercises
   e9e6cbb..14fbe25  master     -> origin/master
Merge made by the 'ort' strategy.
 README.md | 147 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 1 file changed, 147 insertions(+)

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git push origin master
Enumerating objects: 9, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 4 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (5/5), 641 bytes | 213.00 KiB/s, done.
Total 5 (delta 3), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (3/3), completed with 3 local objects.
To https://github.com/Hassanadelani1/gym-GIT-exercises.git
   14fbe25..941e610  master -> master

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git push git-copy master
Enumerating objects: 53, done.
Counting objects: 100% (53/53), done.
Delta compression using up to 4 threads
Compressing objects: 100% (49/49), done.
Writing objects: 100% (53/53), 16.95 KiB | 559.00 KiB/s, done.
Total 53 (delta 26), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (26/26), done.
To https://github.com/Hassanadelani1/git-copy
 * [new branch]      master -> master
```
# Bundle 4
## Excersise 2
```

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git branch ft/footer

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git switch ft/footer
Switched to branch 'ft/footer'

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/footer)
$ ls
README.md  about.html  home.html  services.html  team.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/footer)
$ code team.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/footer)
$ git add .

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/footer)
$ git commit -m 'made some changes to team.html'
[ft/footer 1baff81] made some changes to team.html
 1 file changed, 1 insertion(+), 1 deletion(-)

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/footer)
$ code services.html

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/footer)
$ git status
On branch ft/footer
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   services.html

no changes added to commit (use "git add" and/or "git commit -a")

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/footer)
$ git add .

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/footer)
$ git commit -m 'made some changes to the services.html'
[ft/footer aab7710] made some changes to the services.html
 1 file changed, 1 insertion(+), 1 deletion(-)

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/footer)
$ git push
fatal: The current branch ft/footer has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/footer

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/footer)
$  git push --set-upstream origin ft/footer
Enumerating objects: 19, done.
Counting objects: 100% (19/19), done.
Delta compression using up to 4 threads
Compressing objects: 100% (14/14), done.
Writing objects: 100% (14/14), 3.28 KiB | 258.00 KiB/s, done.
Total 14 (delta 8), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (8/8), completed with 5 local objects.
remote:
remote: Create a pull request for 'ft/footer' on GitHub by visiting:
remote:      https://github.com/Hassanadelani1/gym-GIT-exercises/pull/new/ft/footer
remote:
To https://github.com/Hassanadelani1/gym-GIT-exercises.git
 * [new branch]      ft/footer -> ft/footer
branch 'ft/footer' set up to track 'origin/ft/footer'.

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/footer)
$ git push
Everything up-to-date

HP@Hassan MINGW64 ~/gym-GIT-exercises (ft/footer)
$ git switch master
Switched to branch 'master'
Your branch is up to date with 'origin/master'.

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git branch ft/squashing

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git merge --squash ft/footer
Updating 941e610..aab7710
Fast-forward
Squash commit -- not updating HEAD
 services.html | 2 +-
 team.html     | 2 +-
 2 files changed, 2 insertions(+), 2 deletions(-)

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git status
On branch master
Your branch is up to date with 'origin/master'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   services.html
        modified:   team.html


HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git commit -m "footer changes squashing"
[master cd6e8a0] footer changes squashing
 2 files changed, 2 insertions(+), 2 deletions(-)

HP@Hassan MINGW64 ~/gym-GIT-exercises (master)
$ git push origin ft/squashing
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote:
remote: Create a pull request for 'ft/squashing' on GitHub by visiting:
remote:      https://github.com/Hassanadelani1/gym-GIT-exercises/pull/new/ft/squashing
remote:
To https://github.com/Hassanadelani1/gym-GIT-exercises.git
 * [new branch]      ft/squashing -> ft/squashing
```

