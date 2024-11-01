# first-git
Atashi no testo
Lab E@PC-E-31 MINGW64 ~
$ cd /c/xampp/htdocs/

Lab E@PC-E-31 MINGW64 /c/xampp/htdocs
$ ls
applications.html  dashboard/   img/       webalizer/
bitnami.css        favicon.ico  index.php  xampp/

Lab E@PC-E-31 MINGW64 /c/xampp/htdocs
$ ls -lah
total 58K
drwxr-xr-x 1 Lab E 197121    0 Aug 28  2023 ./
drwxr-xr-x 1 Lab E 197121    0 Aug 28  2023 ../
-rw-r--r-- 1 Lab E 197121 3.6K Aug 27  2019 applications.html
-rw-r--r-- 1 Lab E 197121  177 Aug 27  2019 bitnami.css
drwxr-xr-x 1 Lab E 197121    0 Aug 28  2023 dashboard/
-rw-r--r-- 1 Lab E 197121  31K Jul 16  2015 favicon.ico
drwxr-xr-x 1 Lab E 197121    0 Aug 28  2023 img/
-rw-r--r-- 1 Lab E 197121  260 Jul 16  2015 index.php
drwxr-xr-x 1 Lab E 197121    0 Aug 28  2023 webalizer/
drwxr-xr-x 1 Lab E 197121    0 Aug 28  2023 xampp/

Lab E@PC-E-31 MINGW64 /c/xampp/htdocs
$ git clone https://github.com/lilyorlnd/first-git.git
Cloning into 'first-git'...
remote: Enumerating objects: 4, done.
remote: Counting objects: 100% (4/4), done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 4 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Receiving objects: 100% (4/4), done.

Lab E@PC-E-31 MINGW64 /c/xampp/htdocs
$ ls
applications.html  dashboard/   first-git/  index.php   xampp/
bitnami.css        favicon.ico  img/        webalizer/

Lab E@PC-E-31 MINGW64 /c/xampp/htdocs
$ cd first-git

Lab E@PC-E-31 MINGW64 /c/xampp/htdocs/first-git (main)
$ code .

Lab E@PC-E-31 MINGW64 /c/xampp/htdocs/first-git (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        home.html
        style.css

nothing added to commit but untracked files present (use "git add" to track)

Lab E@PC-E-31 MINGW64 /c/xampp/htdocs/first-git (main)
$ git add index.html
fatal: pathspec 'index.html' did not match any files

Lab E@PC-E-31 MINGW64 /c/xampp/htdocs/first-git (main)
$ git add home.html

Lab E@PC-E-31 MINGW64 /c/xampp/htdocs/first-git (main)
$ git add .

Lab E@PC-E-31 MINGW64 /c/xampp/htdocs/first-git (main)
$ git commit -m "Membuat file index html dan css"
Author identity unknown

*** Please tell me who you are.

Run

  git config --global user.email "you@example.com"
  git config --global user.name "Your Name"

to set your account's default identity.
Omit --global to set the identity only in this repository.

fatal: unable to auto-detect email address (got 'Lab E@PC-E-31.(none)')

Lab E@PC-E-31 MINGW64 /c/xampp/htdocs/first-git (main)
$ git config --global user.email "lndsorlando@gmail.com" ^C

Lab E@PC-E-31 MINGW64 /c/xampp/htdocs/first-git (main)
$ git config --global user.email "lndsorlando@gmail.com"

Lab E@PC-E-31 MINGW64 /c/xampp/htdocs/first-git (main)
$ git config --global user.name "lilyorlnd"

Lab E@PC-E-31 MINGW64 /c/xampp/htdocs/first-git (main)
$ git commit -m "membuat html dan css"
[main fa8b8f1] membuat html dan css
 2 files changed, 244 insertions(+)
 create mode 100644 home.html
 create mode 100644 style.css

Lab E@PC-E-31 MINGW64 /c/xampp/htdocs/first-git (main)
$ git push origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 1.78 KiB | 1.78 MiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/lilyorlnd/first-git.git
   73e8b25..fa8b8f1  main -> main

Lab E@PC-E-31 MINGW64 /c/xampp/htdocs/first-git (main)
$ ^C

Lab E@PC-E-31 MINGW64 /c/xampp/htdocs/first-git (main)
$ git pull origin main
From https://github.com/lilyorlnd/first-git
 * branch            main       -> FETCH_HEAD
Already up to date.

Lab E@PC-E-31 MINGW64 /c/xampp/htdocs/first-git (main)
$ git branch kerjaan-2

Lab E@PC-E-31 MINGW64 /c/xampp/htdocs/first-git (main)
$ git branch -v -a
  kerjaan-2           fa8b8f1 membuat html dan css
* main                fa8b8f1 membuat html dan css
  remotes/origin/HEAD -> origin/main
  remotes/origin/main fa8b8f1 membuat html dan css

Lab E@PC-E-31 MINGW64 /c/xampp/htdocs/first-git (main)
$ git switch 'kerjaan-2'
Switched to branch 'kerjaan-2'

Lab E@PC-E-31 MINGW64 /c/xampp/htdocs/first-git (kerjaan-2)
$ git branch -v -a
* kerjaan-2           fa8b8f1 membuat html dan css
  main                fa8b8f1 membuat html dan css
  remotes/origin/HEAD -> origin/main
  remotes/origin/main fa8b8f1 membuat html dan css

Lab E@PC-E-31 MINGW64 /c/xampp/htdocs/first-git (kerjaan-2)
$ git add .

Lab E@PC-E-31 MINGW64 /c/xampp/htdocs/first-git (kerjaan-2)
$ git commit -m "add new file"
[kerjaan-2 297787c] add new file
 1 file changed, 59 insertions(+)
 create mode 100644 kerjaan2.html

Lab E@PC-E-31 MINGW64 /c/xampp/htdocs/first-git (kerjaan-2)
$ git branch -v -a
* kerjaan-2           297787c add new file
  main                fa8b8f1 membuat html dan css
  remotes/origin/HEAD -> origin/main
  remotes/origin/main fa8b8f1 membuat html dan css

Lab E@PC-E-31 MINGW64 /c/xampp/htdocs/first-git (kerjaan-2)
$ git merge kerjaan-2
Already up to date.

Lab E@PC-E-31 MINGW64 /c/xampp/htdocs/first-git (kerjaan-2)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

Lab E@PC-E-31 MINGW64 /c/xampp/htdocs/first-git (main)
$ git merge kerjaan-2
Updating fa8b8f1..297787c
Fast-forward
 kerjaan2.html | 59 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 1 file changed, 59 insertions(+)
 create mode 100644 kerjaan2.html

Lab E@PC-E-31 MINGW64 /c/xampp/htdocs/first-git (main)
$ git push origin main
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 919 bytes | 919.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/lilyorlnd/first-git.git
   fa8b8f1..297787c  main -> main

Lab E@PC-E-31 MINGW64 /c/xampp/htdocs/first-git (main)
$ ^C

Lab E@PC-E-31 MINGW64 /c/xampp/htdocs/first-git (main)
$ ^C

Lab E@PC-E-31 MINGW64 /c/xampp/htdocs/first-git (main)
$ git fetch origin
git checkout 1-membuat-halaman-profil
From https://github.com/lilyorlnd/first-git
 * [new branch]      1-membuat-halaman-profil -> origin/1-membuat-halaman-profil
Switched to a new branch '1-membuat-halaman-profil'
branch '1-membuat-halaman-profil' set up to track 'origin/1-membuat-halaman-prof
il'.

Lab E@PC-E-31 MINGW64 /c/xampp/htdocs/first-git (1-membuat-halaman-profil)
$ git add .

Lab E@PC-E-31 MINGW64 /c/xampp/htdocs/first-git (1-membuat-halaman-profil)
$ git commit -m "membuat halaman profil"
[1-membuat-halaman-profil 57adf69] membuat halaman profil
 1 file changed, 11 insertions(+)
 create mode 100644 profile.html

Lab E@PC-E-31 MINGW64 /c/xampp/htdocs/first-git (1-membuat-halaman-profil)
$ git push origin main 1-membuat-halaman-profil
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 427 bytes | 427.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/lilyorlnd/first-git.git
   297787c..57adf69  1-membuat-halaman-profil -> 1-membuat-halaman-profil

Lab E@PC-E-31 MINGW64 /c/xampp/htdocs/first-git (1-membuat-halaman-profil)
$
