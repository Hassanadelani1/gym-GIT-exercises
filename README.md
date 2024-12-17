This is the README.md file.
#Bundle 1
##Exercise 1
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
