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
