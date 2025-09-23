# Gym-Git-Exercise-Solutions

## questions 

```
Exercise 1

- Create a project folder & initialize git
- Make changes to the project (add files and contents)
- Rename your main branch from `master` to `main` (If your branch name is already `main` then rename it to `master` and then back to `main`)
- Stage your changes and commit them
- Create a Github repo and connect it with your project
- Push your changes to GitHub
- Create a new branch `dev`
- From `dev` create another branch `test`
- Go back to the `dev` branch and delete the `test` branch

Exercise 2

- Create a new `home.html` file, add some html changes and save them
- Stash save your current changes
- Repeat the same process for a new `about.html` page and stash save your changes
- Repeat the same process for a new `team.html` page and stash save your changes
- Using stash pop restore the changes of the `about.html` page
- With the help of an index use stash pop bring back the `home.html` page changes
- Commit the current changes and push them
- Using stash pop restore the changes of the `team.html` page index
- Reset the current changes using git reset and go back to the changes without the `team.html` page
```






## Bundle 1
 
 ### exercises 1 command

 ```
user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git init 
Reinitialized existing Git repository in C:/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions/.git/

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git branch -m master

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (master)
$ git branch -m main

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git add .

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git commit -m "make simple changes in exercises1"
[main 7ec2f71] make simple changes in exercises1
 4 files changed, 18 insertions(+), 29 deletions(-)
 create mode 100644 Bundle1/exercises.html
 delete mode 100644 exercise1-bundle-1/home.html
 delete mode 100644 exercise1-bundle-1/service.html

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git submodule https://github.com/Vainqueur123/Exercises-repo
usage: git submodule [--quiet] [--cached]
   or: git submodule [--quiet] add [-b <branch>] [-f|--force] [--name <name>] [--reference <repository>] [--] <repository> [<path>]
   or: git submodule [--quiet] status [--cached] [--recursive] [--] [<path>...]
   or: git submodule [--quiet] init [--] [<path>...]
   or: git submodule [--quiet] deinit [-f|--force] (--all| [--] <path>...)
   or: git submodule [--quiet] update [--init [--filter=<filter-spec>]] [--remote] [-N|--no-fetch] [-f|--force] [--checkout|--merge|--rebase] [--[no-]recommend-shallow] [--reference <repository>] [--recursive] [--[no-]single-branch] [--] [<path>...]
   or: git submodule [--quiet] set-branch (--default|--branch <branch>) [--] <path>
   or: git submodule [--quiet] set-url [--] <path> <newurl>
   or: git submodule [--quiet] summary [--cached|--files] [--summary-limit <n>] [commit] [--] [<path>...]
   or: git submodule [--quiet] foreach [--recursive] <command>
   or: git submodule [--quiet] sync [--recursive] [--] [<path>...]
   or: git submodule [--quiet] absorbgitdirs [--] [<path>...]

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git add .

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git commit -m "add files"
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git pull
Already up to date.

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git push 
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (5/5), 604 bytes | 151.00 KiB/s, done.
Total 5 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/Vainqueur123/Gym-Git-Exercise-Solutions.git
   ce9e562..7ec2f71  main -> main

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git checkout -b dev
Switched to a new branch 'dev'

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (dev)
$ git checkout -b test
Switched to a new branch 'test'

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (test)
$ git checkout -d test
HEAD is now at 7ec2f71 make simple changes in exercises1

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions ((7ec2f71...))
$ git checkout dev
Switched to branch 'dev'

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (dev)
$ git checkout -d test
HEAD is now at 7ec2f71 make simple changes in exercises1

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions ((7ec2f71...))
$ git checkout dev
M       Bundle1/exercises.html
Switched to branch 'dev'

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (dev)
$ git checkout -d test
M       Bundle1/exercises.html
HEAD is now at 7ec2f71 make simple changes in exercises1

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions ((7ec2f71...))
$ git checkout dev
M       Bundle1/exercises.html
Switched to branch 'dev'

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (dev)
$ git add .

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (dev)
$ git commit -m "add changes"
[dev 60a55fd] add changes
 1 file changed, 2 insertions(+)

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (dev)
$ git push origin dev
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (4/4), 398 bytes | 199.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/Vainqueur123/Gym-Git-Exercise-Solutions/pull/new/dev
remote:
To https://github.com/Vainqueur123/Gym-Git-Exercise-Solutions.git
 * [new branch]      dev -> dev

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (dev)
$ git checkout -d test
HEAD is now at 7ec2f71 make simple changes in exercises1

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions ((7ec2f71...))
$ git checkout dev
Previous HEAD position was 7ec2f71 make simple changes in exercises1
Switched to branch 'dev'

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (dev)
$ git branch -d test
Deleted branch test (was 7ec2f71).

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (dev)
$
```

### exercises 2

```

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (dev)
$ git checkout main
M       README.md
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ 
$
user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git init 
Reinitialized existing Git repository in C:/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions/.git/

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git branch -m master

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (master)
$^Cr@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (dev)2f71...))th>...]ath>...]--checkout|--merge|--re

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git stash 
No local changes to save

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git stash list
stash@{0}: WIP on main: 7ec2f71 make simple changes in exercises1

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git stash about
fatal: subcommand wasn't specified; 'push' can't be assumed due to unexpected token 'about'

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git stash about.html
fatal: subcommand wasn't specified; 'push' can't be assumed due to unexpected token 'about.html'

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git stash <about.html>
bash: syntax error near unexpected token `newline'

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git stash push Bundle1/about.html
error: pathspec ':(prefix:0)Bundle1/about.html' did not match any file(s) known to git
Did you forget to 'git add'?

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git add .

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git stash push Bundle1/about.html
Saved working directory and index state WIP on main: 7ec2f71 make simple changes in exercises1

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git stash push Bundle1/home.html
Saved working directory and index state WIP on main: 7ec2f71 make simple changes in exercises1

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git stash pop Bundle1/about.html
error: Bundle1/about.html is not a valid reference

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git stash list
stash@{0}: WIP on main: 7ec2f71 make simple changes in exercises1
stash@{1}: WIP on main: 7ec2f71 make simple changes in exercises1
stash@{2}: WIP on main: 7ec2f71 make simple changes in exercises1

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git checkout stash@{1}
Note: switching to 'stash@{1}'.

You are in 'detached HEAD' state. You can look around, make experimental
changes and commit them, and you can discard any commits you make in this
state without impacting any branches by switching back to a branch.

If you want to create a new branch to retain commits you create, you may
do so (now or later) by using -c with the switch command. Example:

  git switch -c <new-branch-name>

Or undo this operation with:

  git switch -

Turn off this advice by setting config variable advice.detachedHead to false

HEAD is now at da3dbca WIP on main: 7ec2f71 make simple changes in exercises1

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions ((da3dbca...))
$ git stash push Bundle1/home.html
No local changes to save

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions ((da3dbca...))
$ git stash push Bundle1/home.html
Saved working directory and index state WIP on (no branch): da3dbca WIP on main: 7ec2f71 make simple changes in exercises1

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions ((da3dbca...))
$ git checkout main 
Previous HEAD position was da3dbca WIP on main: 7ec2f71 make simple changes in exercises1
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git checkout stash@{1}
Note: switching to 'stash@{1}'.

You are in 'detached HEAD' state. You can look around, make experimental
changes and commit them, and you can discard any commits you make in this
state without impacting any branches by switching back to a branch.

If you want to create a new branch to retain commits you create, you may
do so (now or later) by using -c with the switch command. Example:

  git switch -c <new-branch-name>

Or undo this operation with:

  git switch -

Turn off this advice by setting config variable advice.detachedHead to false

HEAD is now at 73c9f77 WIP on main: 7ec2f71 make simple changes in exercises1

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions ((73c9f77...))
$ git checkout main
Warning: you are leaving 2 commits behind, not connected to
any of your branches:

  73c9f77 WIP on main: 7ec2f71 make simple changes in exercises1
  14152b6 index on main: 7ec2f71 make simple changes in exercises1

If you want to keep them by creating a new branch, this may be a good time
to do so with:

 git branch <new-branch-name> 73c9f77

Switched to branch 'main'
Your branch is up to date with 'origin/main'.

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git stash list
stash@{0}: WIP on (no branch): da3dbca WIP on main: 7ec2f71 make simple changes in exercises1
stash@{1}: WIP on main: 7ec2f71 make simple changes in exercises1
stash@{2}: WIP on main: 7ec2f71 make simple changes in exercises1
stash@{3}: WIP on main: 7ec2f71 make simple changes in exercises1

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git stash pop stash@{1}
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   Bundle1/home.html

Dropped stash@{1} (73c9f773fe4e49803b5b17e26b1038a34a1b1d6d)

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git stash pop stash@{2}
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   Bundle1/home.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

Dropped stash@{2} (8c5b69fefaa1530bfcfdfcc5f1a557d8811842af)

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git stash push Bundle1/home.html
Saved working directory and index state WIP on main: 7ec2f71 make simple changes in exercises1

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git liat
git: 'liat' is not a git command. See 'git --help'.

The most similar commands are
        clean
        mktag

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git stash list
stash@{0}: WIP on main: 7ec2f71 make simple changes in exercises1
stash@{1}: WIP on (no branch): da3dbca WIP on main: 7ec2f71 make simple changes in exercises1
stash@{2}: WIP on main: 7ec2f71 make simple changes in exercises1

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git stash pop stash@{2}
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   Bundle1/about.html
        new file:   Bundle1/home.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

Dropped stash@{2} (da3dbcaca046c5a5d18be9ec8aa5dda98c65987b)

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git restore --staged
fatal: you must specify path(s) to restore

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git restore --staged .

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git add Bundle1/about.html 

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git commit -m "add about.html omly"
[main 6d07445] add about.html omly
 1 file changed, 22 insertions(+)
 create mode 100644 Bundle1/about.html

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git stash list 
stash@{0}: WIP on main: 7ec2f71 make simple changes in exercises1
stash@{1}: WIP on (no branch): da3dbca WIP on main: 7ec2f71 make simple changes in exercises1

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git stash pop stash@{0}
error: The following untracked working tree files would be overwritten by merge:
        Bundle1/home.html
Please move or remove them before you merge.
Aborting
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        Bundle1/home.html

no changes added to commit (use "git add" and/or "git commit -a")
The stash entry is kept in case you need it again.

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ rm Bundle1/home.html

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git stash pop stash@{0}
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   Bundle1/home.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

Dropped stash@{0} (2aa34d34fa47a7964afcecd83b02dd9f13808b9e)

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git add Bundle1/home.html 

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git commit -m "bring back home"
[main db506aa] bring back home
 1 file changed, 15 insertions(+)
 create mode 100644 Bundle1/home.html

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git reset
Unstaged changes after reset:
M       README.md

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$  git add .

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git commit -m "push all restored changes "
[main 16ff993] push all restored changes
 1 file changed, 176 insertions(+)

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git push 
Enumerating objects: 14, done.
Counting objects: 100% (14/14), done.
Delta compression using up to 16 threads
Compressing objects: 100% (11/11), done.
Writing objects: 100% (11/11), 2.88 KiB | 1.44 MiB/s, done.
Total 11 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), done.
To https://github.com/Vainqueur123/Gym-Git-Exercise-Solutions.git
   7ec2f71..16ff993  main -> main

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$
```
## Bundle 2

### exercises 1
```

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git checkout -b ft/bundle-2
Switched to a new branch 'ft/bundle-2'

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (ft/bundle-2)
$ git add .

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (ft/bundle-2)
$ git commit -m "add services page"
[ft/bundle-2 a844167] add services page
 2 files changed, 327 insertions(+)
 create mode 100644 services.html

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (ft/bundle-2)
$ git push origin ft/bundle-2 
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 16 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 3.73 KiB | 3.73 MiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote: 
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/Vainqueur123/Gym-Git-Exercise-Solutions/pull/new/ft/bundle-2
remote:
To https://github.com/Vainqueur123/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (ft/bundle-2)
$ git check main 
git: 'check' is not a git command. See 'git --help'.

The most similar command is
        checkout

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (ft/bundle-2)
$ git checkout main
error: Your local changes to the following files would be overwritten by checkout:
        README.md
Please commit your changes or stash them before you switch branches.
Aborting

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (ft/bundle-2)
$ git checkout main 
error: Your local changes to the following files would be overwritten by checkout:
        README.md
Please commit your changes or stash them before you switch branches.
Aborting

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (ft/bundle-2)
$ git checkout main
error: Your local changes to the following files would be overwritten by checkout:
        README.md
Please commit your changes or stash them before you switch branches.
Aborting

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (ft/bundle-2)
$ git add .

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (ft/bundle-2)
$ git commit -m "add changes stored in readmme"
[ft/bundle-2 702a0c0] add changes stored in readmme
 1 file changed, 42 insertions(+), 1 deletion(-)

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (ft/bundle-2)
$ git push origin ft/bundle-2 
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 638 bytes | 638.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/Vainqueur123/Gym-Git-Exercise-Solutions.git
   a844167..702a0c0  ft/bundle-2 -> ft/bundle-2

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (ft/bundle-2)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git pull
remote: Enumerating objects: 1, done.
remote: Counting objects: 100% (1/1), done.
remote: Total 1 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (1/1), 903 bytes | 301.00 KiB/s, done.
From https://github.com/Vainqueur123/Gym-Git-Exercise-Solutions
   16ff993..6bbfb9f  main       -> origin/main
Updating 16ff993..6bbfb9f
Fast-forward
 README.md     | 312 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 services.html |  15 +++
 2 files changed, 327 insertions(+)
 create mode 100644 services.html

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git checkout -b ft/service-redesign
Switched to a new branch 'ft/service-redesign'

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (ft/service-redesign)
$ git add .

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (ft/service-redesign)
$ git commit -m "change in services"
[ft/service-redesign 97c053b] change in services
 1 file changed, 5 insertions(+)

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (ft/service-redesign)
$ git push origin ft/service-redesign 
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 372 bytes | 372.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/Vainqueur123/Gym-Git-Exercise-Solutions/pull/new/ft/service-redesign
remote:
To https://github.com/Vainqueur123/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/service-redesign -> ft/service-redesign

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (ft/service-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git add .

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git commit -m "again add changes in the service page "
[main 3410928] again add changes in the service page
 1 file changed, 5 insertions(+)

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git push 
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 402 bytes | 402.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/Vainqueur123/Gym-Git-Exercise-Solutions.git
   6bbfb9f..3410928  main -> main

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (ft/service-redesign)
$ git diff

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (ft/service-redesign)
$ git diff

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (ft/service-redesign)
$ git merge 
fatal: No remote for the current branch.

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (ft/service-redesign)
$ git checkout main 
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git merge ft/service-redesign 
Auto-merging services.html
CONFLICT (content): Merge conflict in services.html
Automatic merge failed; fix conflicts and then commit the result.

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main|MERGING)
$ git merge
error: Merging is not possible because you have unmerged files.
hint: Fix them up in the work tree, and then use 'git add/rm <file>'
hint: as appropriate to mark resolution and make a commit.
fatal: Exiting because of an unresolved conflict.

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main|MERGING)
$ git merge --abort

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git merge ft/service-redesign 
Auto-merging services.html
CONFLICT (content): Merge conflict in services.html
Automatic merge failed; fix conflicts and then commit the result.

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main|MERGING)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

You have unmerged paths.
  (fix conflicts and run "git commit")
  (use "git merge --abort" to abort the merge)

Unmerged paths:
  (use "git add <file>..." to mark resolution)
        both modified:   services.html

no changes added to commit (use "git add" and/or "git commit -a")

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main|MERGING)
$ git add services.html 

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main|MERGING)
$ git commit -m "remove conflicts in service page"
[main 07107ee] remove conflicts in service page

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git push main
fatal: 'main' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git push origin main
To https://github.com/Vainqueur123/Gym-Git-Exercise-Solutions.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/Vainqueur123/Gym-Git-Exercise-Solutions.git'
hint: Updates were rejected because the remote contains work that you do not
hint: have locally. This is usually caused by another repository pushing to
hint: the same ref. If you want to integrate the remote changes, use
hint: 'git pull' before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git pull origin main --rebase
remote: Enumerating objects: 2, done.
remote: Counting objects: 100% (2/2), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 2 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (2/2), 1.74 KiB | 254.00 KiB/s, done.
From https://github.com/Vainqueur123/Gym-Git-Exercise-Solutions
 * branch            main       -> FETCH_HEAD
   3410928..068cda4  main       -> origin/main
Successfully rebased and updated refs/heads/main.

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git push arigin main 
fatal: 'arigin' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git add .

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git commit -m "fix: conflicts and merge"
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$
```