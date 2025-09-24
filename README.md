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

## Questions for bundle 2

```
Exercises 1

- Create a new branch named `ft/bundle-2`
- Add new changes to your project. create a new page named `services.html` and add some changes
- Commit your changes and create a Pull Request against the `main` branch in your github repository
- Request a review and make sure your Pull request gets merged (Look for someone to merge your PR)

Exercise 2

- Checkout your `main` branch and pull the latest changes
- Create a new branch named `ft/service-redesign`
- Add new changes to the `service.html` page
- commit and push them
- create a new PR for your changes
- go back to your `main` branch and add again new changes to your `service.html` page, you can add different changes but make sure to affect the same part(line of code) as you did in the other PR
- Commit and push those changes
- Now go back to the Github PR you had created for the `ft/service-redesign`branch, you will then see that you have conflicts with the `main` branch
- In your project checkout the `ft/service-redesign`branch
- Compare the `ft/service-redesign`with the `main` branch using git diff and observe the changes
- Using git merge, merge the `main` branch with `ft/service-redesign` branch and commit and push you changes again
```

### exercises 1 & exrcises 2 commands used in terminal
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



## buddle 3
## Questions for bundle 3

### exercises 1 & exercises 2

```
user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git pull origin main 
From https://github.com/Vainqueur123/Gym-Git-Exercise-Solutions
 * branch            main       -> FETCH_HEAD
Already up to date.

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git branch -b ft/team-page
error: unknown switch `b'
usage: git branch [<options>] [-r | -a] [--merged] [--no-merged]
   or: git branch [<options>] [-f] [--recurse-submodules] <branch-name> [<start-point>]
   or: git branch [<options>] [-l] [<pattern>...]
   or: git branch [<options>] [-r] (-d | -D) <branch-name>...
   or: git branch [<options>] (-m | -M) [<old-branch>] <new-branch>
   or: git branch [<options>] (-c | -C) [<old-branch>] <new-branch>
   or: git branch [<options>] [-r | -a] [--points-at]
   or: git branch [<options>] [-r | -a] [--format]

Generic options
    -v, --[no-]verbose    show hash and subject, give twice for upstream branch
    -q, --[no-]quiet      suppress informational messages
    -t, --[no-]track[=(direct|inherit)]
                          set branch tracking configuration
    -u, --[no-]set-upstream-to <upstream>
                          change the upstream info
    --[no-]unset-upstream unset the upstream info
    --[no-]color[=<when>] use colored output
    -r, --remotes         act on remote-tracking branches
    --contains <commit>   print only branches that contain the commit
    --no-contains <commit>
                          print only branches that don't contain the commit
    --[no-]abbrev[=<n>]   use <n> digits to display object names

Specific git-branch actions:
    -a, --all             list both remote-tracking and local branches
    -d, --[no-]delete     delete fully merged branch
    -D                    delete branch (even if not merged)
    -m, --[no-]move       move/rename a branch and its reflog
    -M                    move/rename a branch, even if target exists
    --[no-]omit-empty     do not output a newline after empty formatted refs
    -c, --[no-]copy       copy a branch and its reflog
    -C                    copy a branch, even if target exists
    -l, --[no-]list       list branch names
    --[no-]show-current   show current branch name
    --[no-]create-reflog  create the branch's reflog
    --[no-]edit-description
                          edit the description for the branch
    -f, --[no-]force      force creation, move/rename, deletion
    --merged <commit>     print only branches that are merged
    --no-merged <commit>  print only branches that are not merged
    --[no-]column[=<style>]
                          list branches in columns
    --[no-]sort <key>     field name to sort on
    --[no-]points-at <object>
                          print only branches of the object
    -i, --[no-]ignore-case
                          sorting and filtering are case insensitive
    --[no-]recurse-submodules
                          recurse through submodules
    --[no-]format <format>
                          format to use for the output


user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git checkout -b ft/team-page
Switched to a new branch 'ft/team-page'

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (ft/team-page)
$ git add .

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (ft/team-page)
$ git cpmmit -m "feat: describe team "
git: 'cpmmit' is not a git command. See 'git --help'.

The most similar command is
        commit

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (ft/team-page)
$ git commit -m "feat: describe team "
[ft/team-page be6e0b9] feat: describe team
 2 files changed, 22 insertions(+)
 create mode 100644 .vscode/settings.json
 create mode 100644 team.html

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (ft/team-page)
$ git push origin ft/team-page 
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (5/5), 739 bytes | 246.00 KiB/s, done.
Total 5 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote: 
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:
remote:      https://github.com/Vainqueur123/Gym-Git-Exercise-Solutions/pull/new/ft/team-page
remote:
To https://github.com/Vainqueur123/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/team-page -> ft/team-page

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (ft/team-page)
$ git checkout main 
error: Your local changes to the following files would be overwritten by checkout:
        team.html
Please commit your changes or stash them before you switch branches.
Aborting

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (ft/team-page)
$ git add .

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (ft/team-page)
$ git commit 
hint: Waiting for your editor to close the file... unix2dos: converting file C:/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions/.git/COMMIT_EDITMSG to DOS format...
dos2unix: converting file C:/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions/.git/COMMIT_EDITMSG to Unix format...
Aborting commit due to empty commit message.

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (ft/team-page)
$ gi
bash: gi: command not found

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (ft/team-page)
$ git commit -m "add little changes"
[ft/team-page 2602e01] add little changes
 1 file changed, 2 deletions(-)

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (ft/team-page)
$ git checkout main 
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (main)
$ git checkout -b ft/contanct-page
Switched to a new branch 'ft/contanct-page'

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (ft/contanct-page)
$ git checkout ft/team-page 
Switched to branch 'ft/team-page'

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (ft/team-page)
$ git log
commit 2602e018d3285b54d728693708cfb019bb1457b4 (HEAD -> ft/team-page)
Author: Rumanzi <ndamukundavainqueur@gmail.com>
Date:   Wed Sep 24 15:49:16 2025 +0200

    add little changes

commit be6e0b9cdcb87d1a35cd05cb392a9f921f45118f (origin/ft/team-page)
Author: Rumanzi <ndamukundavainqueur@gmail.com>
:
commit 2602e018d3285b54d728693708cfb019bb1457b4 (HEAD -> ft/team-page)
Author: Rumanzi <ndamukundavainqueur@gmail.com>
Date:   Wed Sep 24 15:49:16 2025 +0200

    add little changes

commit be6e0b9cdcb87d1a35cd05cb392a9f921f45118f (origin/ft/team-page)
Author: Rumanzi <ndamukundavainqueur@gmail.com>
:
commit 2602e018d3285b54d728693708cfb019bb1457b4 (HEAD -> ft/team-page)
Author: Rumanzi <ndamukundavainqueur@gmail.com>
Date:   Wed Sep 24 15:49:16 2025 +0200

    add little changes

commit be6e0b9cdcb87d1a35cd05cb392a9f921f45118f (origin/ft/team-page)
Author: Rumanzi <ndamukundavainqueur@gmail.com>
:
commit 2602e018d3285b54d728693708cfb019bb1457b4 (HEAD -> ft/team-page)
Author: Rumanzi <ndamukundavainqueur@gmail.com>
Date:   Wed Sep 24 15:49:16 2025 +0200

    add little changes

commit be6e0b9cdcb87d1a35cd05cb392a9f921f45118f (origin/ft/team-page)
Author: Rumanzi <ndamukundavainqueur@gmail.com>
Date:   Wed Sep 24 15:40:42 2025 +0200

    feat: describe team

commit 4b4af298e45ffc4535216cd6d6d64545b3e67340 (origin/main, origin/HEAD, main, ft/contanct-page)
Author: Rumanzi <ndamukundavainqueur@gmail.com>
Date:   Tue Sep 23 17:53:09 2025 +0200

    add changes in the readme

commit 28a1b07cae787f83344940ceb248084f770e24bc
Author: Rumanzi <ndamukundavainqueur@gmail.com>
Date:   Tue Sep 23 17:20:38 2025 +0200

    add command used in README

commit 068cda4b4ceb14e08cb3044abbdd4d592951571c
Merge: 3410928 eea857f
Author: Vainqueur Ndamukunda <ndamukundavainqueur@gmail.com>
Date:   Tue Sep 23 17:12:10 2025 +0200

    Merge pull request #2 from Vainqueur123/ft/service-redesign

    change in services

commit eea857fae6a552a461bae22429a62e9f088c77b1
Merge: 97c053b 3410928
Author: Vainqueur Ndamukunda <ndamukundavainqueur@gmail.com>
Date:   Tue Sep 23 17:11:59 2025 +0200

    Merge branch 'main' into ft/service-redesign

commit 341092835c030ba0d7e827f2940997903ce097e6
Author: Rumanzi <ndamukundavainqueur@gmail.com>
Date:   Tue Sep 23 17:00:46 2025 +0200

    again add changes in the service page

commit 97c053b605974b1228a41a833879169e6d0c63b6 (origin/ft/service-redesign, ft/service-redesign)
Author: Rumanzi <ndamukundavainqueur@gmail.com>
Date:   Tue Sep 23 16:56:57 2025 +0200

    change in services

commit 6bbfb9ffced89700073ea01d7460b2774e06bf5d
Merge: 16ff993 a844167
Author: Vainqueur Ndamukunda <ndamukundavainqueur@gmail.com>
Date:   Tue Sep 23 16:49:49 2025 +0200

    Merge pull request #1 from Vainqueur123/ft/bundle-2

    add services page

commit a844167199eb0db99f11b97e95011f053d4ca7f8
Author: Rumanzi <ndamukundavainqueur@gmail.com>
Date:   Tue Sep 23 16:37:38 2025 +0200

    add services page

commit 16ff993952b76c1e471115d04db7c8c3458de579
Author: Rumanzi <ndamukundavainqueur@gmail.com>
Date:   Tue Sep 23 16:32:41 2025 +0200

    push all restored changes

commit db506aaaa4b227158f0d1f85604d4ab0af406c96
Author: Rumanzi <ndamukundavainqueur@gmail.com>
Date:   Tue Sep 23 16:19:46 2025 +0200

    bring back home

commit 6d0744508d0dd8a97c77fa984efa2d836a7af9f0
Author: Rumanzi <ndamukundavainqueur@gmail.com>
Date:   Tue Sep 23 16:09:51 2025 +0200

    add about.html omly

commit 7ec2f710fc4d27a56d3d4bc79eb7951eeb30ee80
Author: Rumanzi <ndamukundavainqueur@gmail.com>
Date:   Mon Sep 22 15:49:48 2025 +0200

    make simple changes in exercises1

commit ce9e56244a735e9dc8faac6f066cf6d680c5cfb9
Author: Rumanzi <ndamukundavainqueur@gmail.com>
Date:   Thu Sep 18 18:05:14 2025 +0200

    feat: make service page

commit 4b0be68c4abf44d22a8aebc2b17e00ecd08caaa9
Author: Vainqueur Ndamukunda <ndamukundavainqueur@gmail.com>
Date:   Tue Sep 16 14:23:44 2025 +0200

    Initial commit
(END)

    feat: make service page

commit 4b0be68c4abf44d22a8aebc2b17e00ecd08caaa9
Author: Vainqueur Ndamukunda <ndamukundavainqueur@gmail.com>
Date:   Tue Sep 16 14:23:44 2025 +0200

    Initial commit
(END)

    feat: make service page

commit 4b0be68c4abf44d22a8aebc2b17e00ecd08caaa9
Author: Vainqueur Ndamukunda <ndamukundavainqueur@gmail.com>
Date:   Tue Sep 16 14:23:44 2025 +0200

    Initial commit
commit 2602e018d3285b54d728693708cfb019bb1457b4 (HEAD -> ft/team-page)
Author: Rumanzi <ndamukundavainqueur@gmail.com>
Date:   Wed Sep 24 15:49:16 2025 +0200

    add little changes

commit be6e0b9cdcb87d1a35cd05cb392a9f921f45118f (origin/ft/team-page)
Author: Rumanzi <ndamukundavainqueur@gmail.com>
...skipping...


                   SUMMARY OF LESS COMMANDS

      Commands marked with * may be preceded by a number, N.
      Notes in parentheses indicate the behavior if N is given.
      A key preceded by a caret indicates the Ctrl key; thus ^K is ctrl-K.

  h  H                 Display this help.
  q  :q  Q  :Q  ZZ     Exit.
 ---------------------------------------------------------------------------

                           MOVING

  e  ^E  j  ^N  CR  *  Forward  one line   (or N lines).
  y  ^Y  k  ^K  ^P  *  Backward one line   (or N lines).
  ESC-j             *  Forward  one file line (or N file lines).
  ESC-k             *  Backward one file line (or N file lines).
  f  ^F  ^V  SPACE  *  Forward  one window (or N lines).
  b  ^B  ESC-v      *  Backward one window (or N lines).
  z                 *  Forward  one window (and set window to N).
  w                 *  Backward one window (and set window to N).
  ESC-SPACE         *  Forward  one window, but don't stop at end-of-file.
  ESC-b             *  Backward one window, but don't stop at beginning-of-file.
  d  ^D             *  Forward  one half-window (and set half-window to N).
  u  ^U             *  Backward one half-window (and set half-window to N).
  ESC-)  RightArrow *  Right one half screen width (or N positions).
  ESC-(  LeftArrow  *  Left  one half screen width (or N positions).
  ESC-}  ^RightArrow   Right to last column displayed.
  ESC-{  ^LeftArrow    Left  to first column.
  F                    Forward forever; like "tail -f".
  ESC-F                Like F but stop when search pattern is found.
  r  ^R  ^L            Repaint screen.
  R                    Repaint screen, discarding buffered input.
        ---------------------------------------------------
        Default "window" is the screen height.
        Default "half-window" is half of the screen height.
 ---------------------------------------------------------------------------

                          SEARCHING

  /pattern          *  Search forward for (N-th) matching line.
  ?pattern          *  Search backward for (N-th) matching line.
  n                 *  Repeat previous search (for N-th occurrence).
  N                 *  Repeat previous search in reverse direction.
  ESC-n             *  Repeat previous search, spanning files.
  ESC-N             *  Repeat previous search, reverse dir. & spanning files.
  ^O^N  ^On         *  Search forward for (N-th) OSC8 hyperlink.
  ^O^P  ^Op         *  Search backward for (N-th) OSC8 hyperlink.
  ^O^L  ^Ol            Jump to the currently selected OSC8 hyperlink.
  ESC-u                Undo (toggle) search highlighting.
  ESC-U                Clear search highlighting.
  &pattern          *  Display only matching lines.
        ---------------------------------------------------
                Search is case-sensitive unless changed with -i or -I.
        A search pattern may begin with one or more of:
        ^N or !  Search for NON-matching lines.
        ^E or *  Search multiple files (pass thru END OF FILE).
        ^F or @  Start search at FIRST file (for /) or last file (for ?).
        ^K       Highlight matches, but don't move (KEEP position).
        ^R       Don't use REGULAR EXPRESSIONS.
        ^S n     Search for match in n-th parenthesized subpattern.
        ^W       WRAP search if no match found.
        ^L       Enter next character literally into pattern.
 ---------------------------------------------------------------------------

                           JUMPING

  g  <  ESC-<       *  Go to first line in file (or line N).
  G  >  ESC->       *  Go to last line in file (or line N).
  p  %              *  Go to beginning of file (or N percent into file).
  t                 *  Go to the (N-th) next tag.
  T                 *  Go to the (N-th) previous tag.
  {  (  [           *  Find close bracket } ) ].
  }  )  ]           *  Find open bracket { ( [.
  ESC-^F <c1> <c2>  *  Find close bracket <c2>.
  ESC-^B <c1> <c2>  *  Find open bracket <c1>.
        ---------------------------------------------------
        Each "find close bracket" command goes forward to the close bracket
          matching the (N-th) open bracket in the top line.
        Each "find open bracket" command goes backward to the open bracket
          matching the (N-th) close bracket in the bottom line.

  m<letter>            Mark the current top line with <letter>.
  M<letter>            Mark the current bottom line with <letter>.
  '<letter>            Go to a previously marked position.
  ''                   Go to the previous position.
  ^X^X                 Same as '.
  ESC-m<letter>        Clear a mark.
        ---------------------------------------------------
        A mark is any upper-case or lower-case letter.
        Certain marks are predefined:
             ^  means  beginning of the file
             $  means  end of the file
 ---------------------------------------------------------------------------

                        CHANGING FILES

  :e [file]            Examine a new file.
  ^X^V                 Same as :e.
  :n                *  Examine the (N-th) next file from the command line.
  :p                *  Examine the (N-th) previous file from the command line.
  :x                *  Examine the first (or N-th) file from the command line.
  ^O^O                 Open the currently selected OSC8 hyperlink.
  :d                   Delete the current file from the command line list.
  =  ^G  :f            Print current file name.
 ---------------------------------------------------------------------------

                    MISCELLANEOUS COMMANDS

  -<flag>              Toggle a command line option [see OPTIONS below].
  --<name>             Toggle a command line option, by name.
  _<flag>              Display the setting of a command line option.
  __<name>             Display the setting of an option, by name.
  +cmd                 Execute the less cmd each time a new file is examined.

  !command             Execute the shell command with $SHELL.
  #command             Execute the shell command, expanded like a prompt.
  |Xcommand            Pipe file between current pos & mark X to shell command.
  s file               Save input to a file.
  v                    Edit the current file with $VISUAL or $EDITOR.
  V                    Print version number of "less".
 ---------------------------------------------------------------------------

                           OPTIONS

        Most options may be changed either on the command line,
        or from within less by using the - or -- command.
        Options may be given in one of two forms: either a single
        character preceded by a -, or a name preceded by --.

  -?  ........  --help
                  Display help (from command line).
  -a  ........  --search-skip-screen
                  Search skips current screen.
  -A  ........  --SEARCH-SKIP-SCREEN
                  Search starts just after target line.
  -b [N]  ....  --buffers=[N]
                  Number of buffers.
  -B  ........  --auto-buffers
                  Don't automatically allocate buffers for pipes.
  -c  ........  --clear-screen
                  Repaint by clearing rather than scrolling.
  -d  ........  --dumb
                  Dumb terminal.
  -D xcolor  .  --color=xcolor
                  Set screen colors.
  -e  -E  ....  --quit-at-eof  --QUIT-AT-EOF
                  Quit at end of file.
  -f  ........  --force
                  Force open non-regular files.
  -F  ........  --quit-if-one-screen
                  Quit if entire file fits on first screen.
  -g  ........  --hilite-search
                  Highlight only last match for searches.
  -G  ........  --HILITE-SEARCH
                  Don't highlight any matches for searches.
  -h [N]  ....  --max-back-scroll=[N]
                  Backward scroll limit.
  -i  ........  --ignore-case
                  Ignore case in searches that do not contain uppercase.
  -I  ........  --IGNORE-CASE
                  Ignore case in all searches.
  -j [N]  ....  --jump-target=[N]
                  Screen position of target lines.
  -J  ........  --status-column
                  Display a status column at left edge of screen.
  -k file  ...  --lesskey-file=file
                  Use a compiled lesskey file.
  -K  ........  --quit-on-intr
                  Exit less in response to ctrl-C.
  -L  ........  --no-lessopen
                  Ignore the LESSOPEN environment variable.
  -m  -M  ....  --long-prompt  --LONG-PROMPT
                  Set prompt style.
  -n .........  --line-numbers
                  Suppress line numbers in prompts and messages.
  -N .........  --LINE-NUMBERS
                  Display line number at start of each line.
  -o [file] ..  --log-file=[file]
                  Copy to log file (standard input only).
  -O [file] ..  --LOG-FILE=[file]
                  Copy to log file (unconditionally overwrite).
  -p pattern .  --pattern=[pattern]
                  Start at pattern (from command line).
  -P [prompt]   --prompt=[prompt]
                  Define new prompt.
  -q  -Q  ....  --quiet  --QUIET  --silent --SILENT
                  Quiet the terminal bell.
  -r  -R  ....  --raw-control-chars  --RAW-CONTROL-CHARS
                  Output "raw" control characters.
  -s  ........  --squeeze-blank-lines
                  Squeeze multiple blank lines.
  -S  ........  --chop-long-lines
                  Chop (truncate) long lines rather than wrapping.
  -t tag  ....  --tag=[tag]
                  Find a tag.
  -T [tagsfile] --tag-file=[tagsfile]
                  Use an alternate tags file.
  -u  -U  ....  --underline-special  --UNDERLINE-SPECIAL
                  Change handling of backspaces, tabs and carriage returns.
  -V  ........  --version
                  Display the version number of "less".
  -w  ........  --hilite-unread
                  Highlight first new line after forward-screen.
  -W  ........  --HILITE-UNREAD
                  Highlight first new line after any forward movement.
  -x [N[,...]]  --tabs=[N[,...]]
                  Set tab stops.
  -X  ........  --no-init
                  Don't use termcap init/deinit strings.
  -y [N]  ....  --max-forw-scroll=[N]
                  Forward scroll limit.
  -z [N]  ....  --window=[N]
                  Set size of window.
  -" [c[c]]  .  --quotes=[c[c]]
                  Set shell quote characters.
  -~  ........  --tilde
                  Don't display tildes after end of file.
  -# [N]  ....  --shift=[N]
                  Set horizontal scroll amount (0 = one half screen width).

                --exit-follow-on-close
                  Exit F command on a pipe when writer closes pipe.
                --file-size
                  Automatically determine the size of the input file.
                --follow-name
                  The F command changes files if the input file is renamed.
                --form-feed
                  Stop scrolling when a form feed character is reached.
                --header=[L[,C[,N]]]
                  Use L lines (starting at line N) and C columns as headers.
                --incsearch
                  Search file as each pattern character is typed in.
                --intr=[C]
                  Use C instead of ^X to interrupt a read.
                --lesskey-context=text
                  Use lesskey source file contents.
                --lesskey-src=file
                  Use a lesskey source file.
                --line-num-width=[N]
                  Set the width of the -N line number field to N characters.
                --match-shift=[N]
                  Show at least N characters to the left of a search match.
                --modelines=[N]
                  Read N lines from the input file and look for vim modelines.
                --mouse
                  Enable mouse input.
                --no-edit-warn
                  Don't warn when using v command on a file opened via LESSOPEN.
                --no-keypad
                  Don't send termcap keypad init/deinit strings.
                --no-histdups
                  Remove duplicates from command history.
                --no-number-headers
                  Don't give line numbers to header lines.
                --no-paste
                  Ignore pasted input.
                --no-search-header-lines
                  Searches do not include header lines.
                --no-search-header-columns
                  Searches do not include header columns.
                --no-search-headers
                  Searches do not include header lines or columns.
                --no-vbell
HELP -- Press RETURN for more, or q when done



user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (ft/team-page)
$ git checkout ft/contanct-page 
M       README.md
Switched to branch 'ft/contanct-page'

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (ft/contanct-page)
$ git checkout ft/team-page 
M       README.md
Switched to branch 'ft/team-page'

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (ft/team-page)
$ git log ft/team-page -1
commit 2602e018d3285b54d728693708cfb019bb1457b4 (HEAD -> ft/team-page)
Author: Rumanzi <ndamukundavainqueur@gmail.com>
Date:   Wed Sep 24 15:49:16 2025 +0200

    add little changes

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (ft/team-page)
$ git checkout ft/contanct-page
M       README.md
Switched to branch 'ft/contanct-page'

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (ft/contanct-page)
$ git add .

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (ft/contanct-page)
$ git commit -m "make changes froom team page"
[ft/contanct-page acd7f2a] make changes froom team page
 1 file changed, 568 insertions(+)

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (ft/contanct-page)
$ git push origin ft/contanct-page 
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 6.99 KiB | 2.33 MiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/contanct-page' on GitHub by visiting:
remote:      https://github.com/Vainqueur123/Gym-Git-Exercise-Solutions/pull/new/ft/contanct-page
remote:
To https://github.com/Vainqueur123/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/contanct-page -> ft/contanct-page

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (ft/contanct-page)
$ git checkout -b ft/faq-page
Switched to a new branch 'ft/faq-page'

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (ft/faq-page)
$ git add .

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (ft/faq-page)
$ git commit -m "create faq page "
[ft/faq-page cb4195d] create faq page
 1 file changed, 17 insertions(+)
 create mode 100644 faq.html

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (ft/faq-page)
$ git push origin ft/faq-page 
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 709 bytes | 354.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote: 
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote:      https://github.com/Vainqueur123/Gym-Git-Exercise-Solutions/pull/new/ft/faq-page
remote:
To https://github.com/Vainqueur123/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/faq-page -> ft/faq-page

user@NSANZABAGANWA MINGW64 /c/Gym Git Exercise Solutions/Gym-Git-Exercise-Solutions (ft/faq-page)
$ git log ft/team-page 
commit 2602e018d3285b54d728693708cfb019bb1457b4 (ft/team-page)
Author: Rumanzi <ndamukundavainqueur@gmail.com>
Date:   Wed Sep 24 15:49:16 2025 +0200

    add little changes

commit be6e0b9cdcb87d1a35cd05cb392a9f921f45118f (origin/ft/team-page)
Author: Rumanzi <ndamukundavainqueur@gmail.com>
Date:   Wed Sep 24 15:40:42 2025 +0200

    feat: describe team

commit 4b4af298e45ffc4535216cd6d6d64545b3e67340 (origin/main, origin/HEAD, main)
:

```