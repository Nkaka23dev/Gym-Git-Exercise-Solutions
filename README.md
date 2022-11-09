# Gym Git Exercise Solutions 

..This is the GYM exercises for the GYM Rwanda.

## Bundle 1

### exercises 1

...

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises
$ git init
Initialized empty Git repository in C:/Users/TheGym/Desktop/gitExercises/.git/

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (master)
$ git branch -M main

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md

nothing added to commit but untracked files present (use "git add" to track)

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git add .

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git commit -m "First commit"
[main (root-commit) 2925340] First commit
 1 file changed, 8 insertions(+)
 create mode 100644 README.md

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git remote add origin https://github.com/Nkaka23dev/Gym-Git-Exercise-Solutions.git

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git push -u origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 299 bytes | 149.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/Nkaka23dev/Gym-Git-Exercise-Solutions.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git checkout dev 
error: pathspec 'dev' did not match any file(s) known to git

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git checkout -b  dev
Switched to a new branch 'dev'

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git push
fatal: The current branch dev has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin dev

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$  git push --set-upstream origin dev
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/Nkaka23dev/Gym-Git-Exercise-Solutions/pull/new/dev
remote:
To https://github.com/Nkaka23dev/Gym-Git-Exercise-Solutions.git
 * [new branch]      dev -> dev
branch 'dev' set up to track 'origin/dev'.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git checkout -b test
Switched to a new branch 'test'

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (test)
$ git push
fatal: The current branch test has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin test

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (test)
$  git push --set-upstream origin test
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'test' on GitHub by visiting:
remote:      https://github.com/Nkaka23dev/Gym-Git-Exercise-Solutions/pull/new/test
remote:
To https://github.com/Nkaka23dev/Gym-Git-Exercise-Solutions.git
 * [new branch]      test -> test
branch 'test' set up to track 'origin/test'.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (test)
$ git push origin --delete test
To https://github.com/Nkaka23dev/Gym-Git-Exercise-Solutions.git
 - [deleted]         test

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (test)
$ git branch
  dev
  main
* test

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (test)
$ git branch -d test
error: Cannot delete branch 'test' checked out at 'C:/Users/TheGym/Desktop/gitExercises'

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (test)
$ git checkout dev
Switched to branch 'dev'
Your branch is up to date with 'origin/dev'.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git branch -d test
Deleted branch test (was 2925340).

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git branch
* dev
  main

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$
...