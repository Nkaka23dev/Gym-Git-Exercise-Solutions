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

### exercises 2

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
