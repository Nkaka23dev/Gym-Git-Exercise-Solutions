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

### exercises 1

...
TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git status
On branch dev
Your branch is ahead of 'origin/dev' by 1 commit.
  (use "git push" to publish your local commits)

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        home.html

nothing added to commit but untracked files present (use "git add" to track)

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git add home.html

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash
Saved working directory and index state WIP on dev: d748a80 Updaded readMe

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash list
stash@{0}: WIP on dev: d748a80 Updaded readMe

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git status
On branch dev
Your branch is ahead of 'origin/dev' by 1 commit.
  (use "git push" to publish your local commits)

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        about.html

nothing added to commit but untracked files present (use "git add" to track)

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git add .

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash
Saved working directory and index state WIP on dev: d748a80 Updaded readMe

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash list
stash@{0}: WIP on dev: d748a80 Updaded readMe
stash@{1}: WIP on dev: d748a80 Updaded readMe

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git status
On branch dev
Your branch is ahead of 'origin/dev' by 1 commit.
  (use "git push" to publish your local commits)

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        team.html

nothing added to commit but untracked files present (use "git add" to track)

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git add .

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash
Saved working directory and index state WIP on dev: d748a80 Updaded readMe

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash list
stash@{0}: WIP on dev: d748a80 Updaded readMe
stash@{1}: WIP on dev: d748a80 Updaded readMe
stash@{2}: WIP on dev: d748a80 Updaded readMe

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash pop stash@{1}
On branch dev
Your branch is ahead of 'origin/dev' by 1 commit.
  (use "git push" to publish your local commits)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Dropped stash@{1} (357dde07ed0c4bb6c189481d0dcbdcd0a3db64e6)

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash list
stash@{0}: WIP on dev: d748a80 Updaded readMe
stash@{1}: WIP on dev: d748a80 Updaded readMe

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash pop 0
On branch dev
Your branch is ahead of 'origin/dev' by 1 commit.
  (use "git push" to publish your local commits)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   team.html

Dropped refs/stash@{0} (7829b36eba073f5c8a5083bd4059ce9c046dd85a)

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash list
stash@{0}: WIP on dev: d748a80 Updaded readMe

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git status
On branch dev
Your branch is ahead of 'origin/dev' by 1 commit.
  (use "git push" to publish your local commits)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   team.html


TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git add team.html

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash
Saved working directory and index state WIP on dev: d748a80 Updaded readMe

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash list
stash@{0}: WIP on dev: d748a80 Updaded readMe
stash@{1}: WIP on dev: d748a80 Updaded readMe

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git add .

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash
No local changes to save

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash list
stash@{0}: WIP on dev: d748a80 Updaded readMe
stash@{1}: WIP on dev: d748a80 Updaded readMe

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash pop 1
On branch dev
Your branch is ahead of 'origin/dev' by 1 commit.
  (use "git push" to publish your local commits)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   home.html

Dropped refs/stash@{1} (c8943bff9d08ec6397527bc3bbbe1179160ec384)

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash pop 0
On branch dev
Your branch is ahead of 'origin/dev' by 1 commit.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash list

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git status
On branch dev
Your branch is ahead of 'origin/dev' by 1 commit.  
  (use "git push" to publish your local commits)   

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html 
        new file:   team.html 

Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        deleted:    about.html
        modified:   home.html
        deleted:    team.html


TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git add .

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ gitstatus
bash: gitstatus: command not found

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git status

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash
Saved working directory and index state WIP on dev: d748a80 Updaded readMe

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash list
stash@{0}: WIP on dev: d748a80 Updaded readMe

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git status
On branch dev
Your branch is ahead of 'origin/dev' by 1 commit.
  (use "git push" to publish your local commits) 

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        About.html

nothing added to commit but untracked files present (use "git add" to track)

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git add .

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash
Saved working directory and index state WIP on dev: d748a80 Updaded readMe

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash
No local changes to save

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash list
stash@{0}: WIP on dev: d748a80 Updaded readMe
stash@{1}: WIP on dev: d748a80 Updaded readMe

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git status
On branch dev
Your branch is ahead of 'origin/dev' by 1 commit.
  (use "git push" to publish your local commits)

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        Team.html

nothing added to commit but untracked files present (use "git add" to track)

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git add .

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash
Saved working directory and index state WIP on dev: d748a80 Updaded readMe

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash list
stash@{0}: WIP on dev: d748a80 Updaded readMe
stash@{1}: WIP on dev: d748a80 Updaded readMe
stash@{2}: WIP on dev: d748a80 Updaded readMe

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash pop stash@{1}
On branch dev
Your branch is ahead of 'origin/dev' by 1 commit.
  (use "git push" to publish your local commits)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   About.html

Dropped stash@{1} (dd89b145689c5016f468086ac1a6ce0e0699a8ac)

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash list
stash@{0}: WIP on dev: d748a80 Updaded readMe
stash@{1}: WIP on dev: d748a80 Updaded readMe

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash pop 1
On branch dev
Your branch is ahead of 'origin/dev' by 1 commit.
  (use "git push" to publish your local commits)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   About.html
        new file:   home.html

Dropped refs/stash@{1} (b8d8895eabbda21d6b5c032c3c81701d1917b746)

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git commit -m "bring back stashed file home and abou"
[dev bcc905a] bring back stashed file home and abou
 2 files changed, 24 insertions(+)
 create mode 100644 About.html
 create mode 100644 home.html

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git push
Enumerating objects: 9, done.
Counting objects: 100% (9/9), done.
Delta compression using up to 4 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (7/7), 1.88 KiB | 384.00 KiB/s, done.
Total 7 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/Nkaka23dev/Gym-Git-Exercise-Solutions.git
   2925340..bcc905a  dev -> dev

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash pop
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   Team.html

Dropped refs/stash@{0} (c3f5dd48f95f9b910d769e23b92961a85c99c54b)

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git reset

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git log
commit bcc905a9a6b64dd285c213afa8ff9b9c0d6e7dce (HEAD -> dev, origin/dev)
Author: Nkaka23dev <nkakaeric96@gmail.com>
Date:   Wed Nov 9 17:44:50 2022 +0200

    bring back stashed file home and abou

commit d748a80f787230d8138d92a3c086eb801e3d3d6d
Author: Nkaka23dev <nkakaeric96@gmail.com>
Date:   Wed Nov 9 17:20:45 2022 +0200

    Updaded readMe

commit 2925340d569dd5dd4ac8a1af22213bf13b1f29e0 (origin/main, main)
Author: Nkaka23dev <nkakaeric96@gmail.com>
Date:   Wed Nov 9 17:15:02 2022 +0200
...skipping...
commit bcc905a9a6b64dd285c213afa8ff9b9c0d6e7dce (HEAD -> dev, origin/dev)
Author: Nkaka23dev <nkakaeric96@gmail.com>
Date:   Wed Nov 9 17:44:50 2022 +0200

    bring back stashed file home and abou

commit d748a80f787230d8138d92a3c086eb801e3d3d6d
Author: Nkaka23dev <nkakaeric96@gmail.com>
Date:   Wed Nov 9 17:20:45 2022 +0200

    Updaded readMe

commit 2925340d569dd5dd4ac8a1af22213bf13b1f29e0 (origin/main, main)
Author: Nkaka23dev <nkakaeric96@gmail.com>
Date:   Wed Nov 9 17:15:02 2022 +0200


TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git log
commit bcc905a9a6b64dd285c213afa8ff9b9c0d6e7dce (HEAD -> dev, origin/dev)
Author: Nkaka23dev <nkakaeric96@gmail.com>
Date:   Wed Nov 9 17:44:50 2022 +0200

    bring back stashed file home and abou

commit d748a80f787230d8138d92a3c086eb801e3d3d6d
Author: Nkaka23dev <nkakaeric96@gmail.com>
Date:   Wed Nov 9 17:20:45 2022 +0200

    Updaded readMe

commit 2925340d569dd5dd4ac8a1af22213bf13b1f29e0 (origin/main, main)
Author: Nkaka23dev <nkakaeric96@gmail.com>
Date:   Wed Nov 9 17:15:02 2022 +0200

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git reset --hard bcc905a9a6b64dd285c213afa8ff9b9c0d6e7dce1~
fatal: ambiguous argument 'bcc905a9a6b64dd285c213afa8ff9b9c0d6e7dce1~': unknown revision or path not in the working tree.
Use '--' to separate paths from revisions, like this:
'git <command> [<revision>...] -- [<file>...]'

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git reset --hard 'bcc905a9a6b64dd285c213afa8ff9b9c0d6e7dce1'
fatal: ambiguous argument 'bcc905a9a6b64dd285c213afa8ff9b9c0d6e7dce1': unknown revision or path not in the working tree.
Use '--' to separate paths from revisions, like this:
'git <command> [<revision>...] -- [<file>...]'

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git reset --hard bcc905a9a6b64dd285c213afa8ff9b9c0d6e7dce1
fatal: ambiguous argument 'bcc905a9a6b64dd285c213afa8ff9b9c0d6e7dce1': unknown revision or path not in the working tree.
Use '--' to separate paths from revisions, like this:
'git <command> [<revision>...] -- [<file>...]'

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git restore d748a80f787230d8138d92a3c086eb801e3d3d6d1~
error: pathspec 'd748a80f787230d8138d92a3c086eb801e3d3d6d1~' did not match any file(s) known to git

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git restore d748a80f787230d8138d92a3c086eb801e3d3d6d1
error: pathspec 'd748a80f787230d8138d92a3c086eb801e3d3d6d1' did not match any file(s) known to 
git

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git reset  d748a80f787230d8138d92a3c086eb801e3d3d6d1
fatal: ambiguous argument 'd748a80f787230d8138d92a3c086eb801e3d3d6d1': unknown revision or path not in the working tree.
Use '--' to separate paths from revisions, like this:
'git <command> [<revision>...] -- [<file>...]'

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git reset --hard
HEAD is now at bcc905a bring back stashed file home and abou

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git add team.html

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash 
No local changes to save

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash list

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git status
On branch dev
Your branch is up to date with 'origin/dev'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        Team.html

nothing added to commit but untracked files present (use "git add" to track)

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git add .

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash
Saved working directory and index state WIP on dev: bcc905a bring back stashed file home and abou

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash list
stash@{0}: WIP on dev: bcc905a bring back stashed file home and abou

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash pop
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   Team.html

Dropped refs/stash@{0} (dc6af4fd1c44fef4a298d0cddf32857c27f4c86c)

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git reset --hard
HEAD is now at bcc905a bring back stashed file home and abou

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$
...

## Bundle 1

### exercises 1

...
TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git add .

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git commit -m "Bundle 1 exercise 2 DONE111"
[dev acef7a1] Bundle 1 exercise 2 DONE111
 1 file changed, 465 insertions(+), 1 deletion(-)

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git status
On branch dev
Your branch is ahead of 'origin/dev' by 1 commit.
  (use "git push" to publish your local commits)


TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/bundle-2)
$ git status
On branch ft/bundle-2
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        services.html

nothing added to commit but untracked files present (use "git add" to track)

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/bundle-2)
$ git add .

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/bundle-2)
$ git commit -m "added services page"
[ft/bundle-2 8ad5ea0] added services page
 1 file changed, 12 insertions(+)
 create mode 100644 services.html

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/bundle-2)
$ git push
fatal: The current branch ft/bundle-2 has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/bundle-2

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/bundle-2)
$ git push --set-upstream origin ft/bundle-2
Enumerating objects: 15, done.
Counting objects: 100% (15/15), done.
Delta compression using up to 4 threads
Compressing objects: 100% (12/12), done.
Writing objects: 100% (13/13), 3.77 KiB | 966.00 KiB/s, done.
Total 13 (delta 4), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (4/4), done.
remote:
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/Nkaka23dev/Gym-Git-Exercise-Solutions/pull/new/ft/bundle-2     
remote:
To https://github.com/Nkaka23dev/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2
branch 'ft/bundle-2' set up to track 'origin/ft/bundle-2'.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/service-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   services.html

no changes added to commit (use "git add" and/or "git commit -a")

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git add --all

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git commit -m services on main"
> ^C

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git commit -m 'services on main"
> ^C

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git sttaus
git: 'sttaus' is not a git command. See 'git --help'.

The most similar command is
        status

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   services.html


TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git commit -m "changed services form main"
[main b279826] changed services form main
 1 file changed, 1 insertion(+)

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git branch
  dev
  ft/bundle-2
  ft/service-redesign
* main

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'
Your branch is up to date with 'origin/ft/service-redesign'.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/service-redesign)
$ git merge main
Auto-merging services.html
CONFLICT (content): Merge conflict in services.html
Automatic merge failed; fix conflicts and then commit the result.
TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/service-redesign|MERGING)
$ git add .

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/service-redesign|MERGING)
$ git commit -m "updated"
[ft/service-redesign f13ae85] updated

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/service-redesign)
$
... 


## Bundle 3

### exercises 1

...

...