SAPCT@CC-PC090 MINGW64 /d
$ git clone https://github.com/varun7537/GitPractical.git
Cloning into 'GitPractical'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Receiving objects: 100% (3/3), done.

SAPCT@CC-PC090 MINGW64 /d
$ cd GitPractical

SAPCT@CC-PC090 MINGW64 /d/GitPractical (main)
$ git remote add origin https://github.com/varun7537/GitPractical.git
error: remote origin already exists.

SAPCT@CC-PC090 MINGW64 /d/GitPractical (main)
$ git checkout -b mynewgitbranch
Switched to a new branch 'mynewgitbranch'

SAPCT@CC-PC090 MINGW64 /d/GitPractical (mynewgitbranch)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

SAPCT@CC-PC090 MINGW64 /d/GitPractical (main)
$ git pull origin main
From https://github.com/varun7537/GitPractical
 * branch            main       -> FETCH_HEAD
Already up to date.

SAPCT@CC-PC090 MINGW64 /d/GitPractical (main)
$ git merge mynewgitbranch
Already up to date.

SAPCT@CC-PC090 MINGW64 /d/GitPractical (main)
$ touch index.html

SAPCT@CC-PC090 MINGW64 /d/GitPractical (main)
$ touch style.css

SAPCT@CC-PC090 MINGW64 /d/GitPractical (main)
$ touch script.js

SAPCT@CC-PC090 MINGW64 /d/GitPractical (main)
$ ls
README.md  index.html  script.js  style.css

SAPCT@CC-PC090 MINGW64 /d/GitPractical (main)
$ git add --all

SAPCT@CC-PC090 MINGW64 /d/GitPractical (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   index.html
        new file:   script.js
        new file:   style.css


SAPCT@CC-PC090 MINGW64 /d/GitPractical (main)
$ git commit -m "added new files"
[main 3709693] added new files
 3 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 index.html
 create mode 100644 script.js
 create mode 100644 style.css

SAPCT@CC-PC090 MINGW64 /d/GitPractical (main)
$ git push origin main
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 12 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 301 bytes | 301.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/varun7537/GitPractical.git
   4fa4a20..3709693  main -> main

SAPCT@CC-PC090 MINGW64 /d/GitPractical (main)
$ git pull origin main
From https://github.com/varun7537/GitPractical
 * branch            main       -> FETCH_HEAD
Already up to date.

SAPCT@CC-PC090 MINGW64 /d/GitPractical (main)
$ git merge mynewgitbranch
Already up to date.

SAPCT@CC-PC090 MINGW64 /d/GitPractical (main)
$ git checkout
Your branch is up to date with 'origin/main'.

SAPCT@CC-PC090 MINGW64 /d/GitPractical (main)
$ git checkout mynewgitbranch
Switched to branch 'mynewgitbranch'

SAPCT@CC-PC090 MINGW64 /d/GitPractical (mynewgitbranch)
$ touch new-index.html

SAPCT@CC-PC090 MINGW64 /d/GitPractical (mynewgitbranch)
$ touch new-index.css

SAPCT@CC-PC090 MINGW64 /d/GitPractical (mynewgitbranch)
$ touch new-index.js

SAPCT@CC-PC090 MINGW64 /d/GitPractical (mynewgitbranch)
$ git add --all

SAPCT@CC-PC090 MINGW64 /d/GitPractical (mynewgitbranch)
$ git status
On branch mynewgitbranch
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   new-index.css
        new file:   new-index.html
        new file:   new-index.js


SAPCT@CC-PC090 MINGW64 /d/GitPractical (mynewgitbranch)
$ git commit -m "files are added"
[mynewgitbranch 25c2705] files are added
 3 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 new-index.css
 create mode 100644 new-index.html
 create mode 100644 new-index.js

SAPCT@CC-PC090 MINGW64 /d/GitPractical (mynewgitbranch)
$ git push
fatal: The current branch mynewgitbranch has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin mynewgitbranch

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


SAPCT@CC-PC090 MINGW64 /d/GitPractical (mynewgitbranch)
$ git push origin mynewgitbranch
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 12 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 295 bytes | 295.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote:
remote: Create a pull request for 'mynewgitbranch' on GitHub by visiting:
remote:      https://github.com/varun7537/GitPractical/pull/new/mynewgitbranch
remote:
To https://github.com/varun7537/GitPractical.git
 * [new branch]      mynewgitbranch -> mynewgitbranch

