GIT EXERCISES 

BUNDLE 1
=======
EXERCISES 1
***********
LENOVO@DESKTOP-5GQ3HIK MINGW64 ~/Desktop/TheGym/Git-EXERCISE_SOLUTION (main)
$ git init
Reinitialized existing Git repository in C:/Users/LENOVO/Desktop/TheGym/Git-EXERCISE_SOLUTION/.git/

LENOVO@DESKTOP-5GQ3HIK MINGW64 ~/Desktop/TheGym/Git-EXERCISE_SOLUTION (main)
$ git branch -m master main
error: refname refs/heads/master not found
fatal: Branch rename failed

LENOVO@DESKTOP-5GQ3HIK MINGW64 ~/Desktop/TheGym/Git-EXERCISE_SOLUTION (main)
$ touch README.md

LENOVO@DESKTOP-5GQ3HIK MINGW64 ~/Desktop/TheGym/Git-EXERCISE_SOLUTION (main)
$ git add .

LENOVO@DESKTOP-5GQ3HIK MINGW64 ~/Desktop/TheGym/Git-EXERCISE_SOLUTION (main)
$ git commit -m 'added readme file'
[main (root-commit) 0290ff9] added readme file
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 README.md

LENOVO@DESKTOP-5GQ3HIK MINGW64 ~/Desktop/TheGym/Git-EXERCISE_SOLUTION (main)
$ git push - u origin main
error: src refspec u does not match any
error: src refspec origin does not match any
error: failed to push some refs to '-'

LENOVO@DESKTOP-5GQ3HIK MINGW64 ~/Desktop/TheGym/Git-EXERCISE_SOLUTION (main)
$ git push -u origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 215 bytes | 107.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/gitarecy/Git-EXERCISE_SOLUTION.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

LENOVO@DESKTOP-5GQ3HIK MINGW64 ~/Desktop/TheGym/Git-EXERCISE_SOLUTION (main)
$ git branch -b dev
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
    -v, --verbose         show hash and subject, give twice for upstream branch
    -q, --quiet           suppress informational messages
    -t, --track[=(direct|inherit)]
                          set branch tracking configuration
    -u, --set-upstream-to <upstream>
                          change the upstream info
    --unset-upstream      unset the upstream info
    --color[=<when>]      use colored output
    -r, --remotes         act on remote-tracking branches
    --contains <commit>   print only branches that contain the commit
    --no-contains <commit>
                          print only branches that don't contain the commit
    --abbrev[=<n>]        use <n> digits to display object names

Specific git-branch actions:
    -a, --all             list both remote-tracking and local branches
    -d, --delete          delete fully merged branch
    -D                    delete branch (even if not merged)
    -m, --move            move/rename a branch and its reflog
    -M                    move/rename a branch, even if target exists
    -c, --copy            copy a branch and its reflog
    -C                    copy a branch, even if target exists
    -l, --list            list branch names
    --show-current        show current branch name
    --create-reflog       create the branch's reflog
    --edit-description    edit the description for the branch
    -f, --force           force creation, move/rename, deletion
    --merged <commit>     print only branches that are merged
    --no-merged <commit>  print only branches that are not merged
    --column[=<style>]    list branches in columns
    --sort <key>          field name to sort on
    --points-at <object>  print only branches of the object
    -i, --ignore-case     sorting and filtering are case insensitive
    --recurse-submodules  recurse through submodules
    --format <format>     format to use for the output


LENOVO@DESKTOP-5GQ3HIK MINGW64 ~/Desktop/TheGym/Git-EXERCISE_SOLUTION (main)
$ git branch dev

LENOVO@DESKTOP-5GQ3HIK MINGW64 ~/Desktop/TheGym/Git-EXERCISE_SOLUTION (main)
$ git checkout dev
Switched to branch 'dev'

LENOVO@DESKTOP-5GQ3HIK MINGW64 ~/Desktop/TheGym/Git-EXERCISE_SOLUTION (dev)
$ git checkout -b test
Switched to a new branch 'test'

LENOVO@DESKTOP-5GQ3HIK MINGW64 ~/Desktop/TheGym/Git-EXERCISE_SOLUTION (test)
$ touch text.txt

LENOVO@DESKTOP-5GQ3HIK MINGW64 ~/Desktop/TheGym/Git-EXERCISE_SOLUTION (test)
$ git checkout dev
Switched to branch 'dev'

LENOVO@DESKTOP-5GQ3HIK MINGW64 ~/Desktop/TheGym/Git-EXERCISE_SOLUTION (dev)
$ git branch -d test
Deleted branch test (was 0290ff9).

LENOVO@DESKTOP-5GQ3HIK MINGW64 ~/Desktop/TheGym/Git-EXERCISE_SOLUTION (dev)
$
