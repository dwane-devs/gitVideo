
git init

git add . <- is what we want to save -- now in to the staging area

git commit -m "my message"


dwanepennant@Dwanes-MacBook-Pro gitVideo % git log
commit 5e14826ba9f58b4144e536afb8fe07bcf3d38f73 (HEAD -> master)
Author: Itchy Panda <Itchy@example.com>
Date:   Mon Apr 25 19:52:24 2022 -0400

    deleted html file added app.js

commit ae4a8dadea9da73adcd787e9a910d3842f82541d
Author: Itchy Panda <Itchy@example.com>
Date:   Mon Apr 25 19:50:37 2022 -0400

    add html and css file

dwanepennant@Dwanes-MacBook-Pro gitVideo % git checkout ae4a8dadea9da73adcd787e9a910d3842f82541d
Note: switching to 'ae4a8dadea9da73adcd787e9a910d3842f82541d'.

You are in 'detached HEAD' state. You can look around, make experimental
changes and commit them, and you can discard any commits you make in this
state without impacting any branches by switching back to a branch.

If you want to create a new branch to retain commits you create, you may
do so (now or later) by using -c with the switch command. Example:

  git switch -c <new-branch-name>

Or undo this operation with:

  git switch -

Turn off this advice by setting config variable advice.dls
etachedHead to falsels


HEAD is now at ae4a8da add html and css file
dwanepennant@Dwanes-MacBook-Pro gitVideo % 


# You are now in a different Branch!!

dwanepennant@Dwanes-MacBook-Pro gitVideo % git branch
* (HEAD detached at ae4a8da)
  master

  How do I get back to the master branch


  ------

  …or create a new repository on the command line
echo "# gitVideo" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/dwane-devs/gitVideo.git
git push -u origin main
…or push an existing repository from the command line
git remote add origin https://github.com/dwane-devs/gitVideo.git
git branch -M main
git push -u origin main
…or import code from another repository
You can initialize this repository with code from a Subversion, Mercurial, or TFS project.

========

dwanepennant@Dwanes-MacBook-Pro gitVideo % git branch -M master
fatal: Invalid branch name: 'HEAD'
dwanepennant@Dwanes-MacBook-Pro gitVideo % git branch
* (HEAD detached from ae4a8da)
  master
dwanepennant@Dwanes-MacBook-Pro gitVideo % git checkout master
Warning: you are leaving 1 commit behind, not connected to
any of your branches:

  945813a added readme

If you want to keep it by creating a new branch, this may be a good time
to do so with:

 git branch <new-branch-name> 945813a

Switched to branch 'master'
dwanepennant@Dwanes-MacBook-Pro gitVideo % echo "# gitVideo" >> README.md
dwanepennant@Dwanes-MacBook-Pro gitVideo % git add . 
dwanepennant@Dwanes-MacBook-Pro gitVideo % git branch -M main
dwanepennant@Dwanes-MacBook-Pro gitVideo % git branch
* main
dwanepennant@Dwanes-MacBook-Pro gitVideo % git remote add origin https://github.com/dwane-devs/gitVideo.git
dwanepennant@Dwanes-MacBook-Pro gitVideo % git push -u origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 10 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (5/5), 435 bytes | 435.00 KiB/s, done.
Total 5 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/dwane-devs/gitVideo.git
 * [new branch]      main -> main
Branch 'main' set up to track remote branch 'main' from 'origin'.
dwanepennant@Dwanes-MacBook-Pro gitVideo % git checkout -b newBranch

========

To create a new branch:
 git checkout -b newBranch

