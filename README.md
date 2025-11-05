
C:\laragon\www
λ mkdir Sigmaa

C:\laragon\www
λ cd Sigmaa

C:\laragon\www\Sigmaa
λ git init
hint: Using 'master' as the name for the initial branch. This default branch name
hint: is subject to change. To configure the initial branch name to use in all
hint: of your new repositories, which will suppress this warning, call:
hint:
hint:   git config --global init.defaultBranch <name>
hint:
hint: Names commonly chosen instead of 'master' are 'main', 'trunk' and
hint: 'development'. The just-created branch can be renamed via this command:
hint:
hint:   git branch -m <name>
Initialized empty Git repository in C:/laragon/www/Sigmaa/.git/

C:\laragon\www\Sigmaa(master)
λ git config --global init.defaultBranch Sigmaa

C:\laragon\www\Sigmaa(master)
λ ls -a
./  ../  .git/

C:\laragon\www\Sigmaa(master)
λ git remote add origin  https://github.com/rinaldsp18-dot/Sigmaa.git

C:\laragon\www\Sigmaa(master)
λ git branch Main
fatal: not a valid object name: 'master'

C:\laragon\www\Sigmaa(master)
λ git branch -M main

C:\laragon\www\Sigmaa(main)
λ git remote remove origin https://github.com/rinaldsp18-dot/Sigmaa.git
usage: git remote remove <name>


C:\laragon\www\Sigmaa(main)
λ git remote remove https://github.com/rinaldsp18-dot/Sigmaa.git
error: No such remote: 'https://github.com/rinaldsp18-dot/Sigmaa.git'

C:\laragon\www\Sigmaa(main)
λ git remote remove origin https://github.com/LiepinsDiepins/Sigmaa.git
usage: git remote remove <name>


C:\laragon\www\Sigmaa(main)
λ git remote add origin https://github.com/LiepinsDiepins/Sigmaa.git
error: remote origin already exists.

C:\laragon\www\Sigmaa(main)
λ touch index.html

C:\laragon\www\Sigmaa(main)
λ git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        index.html

nothing added to commit but untracked files present (use "git add" to track)

C:\laragon\www\Sigmaa(main)
λ git add .

C:\laragon\www\Sigmaa(main)
λ git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   index.html


C:\laragon\www\Sigmaa(main)
λ git commit -m "Pievienots index.html"
[main (root-commit) f37707e] Pievienots index.html
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 index.html

C:\laragon\www\Sigmaa(main)
λ git push
fatal: The current branch main has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin main

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


C:\laragon\www\Sigmaa(main)
λ git push --set-upstream origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 228 bytes | 228.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/rinaldsp18-dot/Sigmaa.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

C:\laragon\www\Sigmaa(main -> origin)
λ ls -a
./  ../  .git/  index.html

C:\laragon\www\Sigmaa(main -> origin)
λ code .

C:\laragon\www\Sigmaa(main -> origin)
λ git add .

C:\laragon\www\Sigmaa(main -> origin)
λ git commit -m "Pieliku sarakstu"
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

C:\laragon\www\Sigmaa(main -> origin)
λ git push
Everything up-to-date

C:\laragon\www\Sigmaa(main -> origin)
λ git add .

C:\laragon\www\Sigmaa(main -> origin)
λ git commit -m "Pieliku sarakstu"
[main eaf92d7] Pieliku sarakstu
 1 file changed, 11 insertions(+)

C:\laragon\www\Sigmaa(main -> origin)
λ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 412 bytes | 412.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/rinaldsp18-dot/Sigmaa.git
   f37707e..eaf92d7  main -> main

C:\laragon\www\Sigmaa(main -> origin)
