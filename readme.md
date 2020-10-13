So basically there are the instructions of what I did in terminal.

dci@dci-Aspire-A515-55:~$ cd Desktop
dci@dci-Aspire-A515-55:~/Desktop$ mkdir extratask
dci@dci-Aspire-A515-55:~/Desktop$ cd extratask
dci@dci-Aspire-A515-55:~/Desktop/extratask$ touch books.md
dci@dci-Aspire-A515-55:~/Desktop/extratask$ touch movies.md
dci@dci-Aspire-A515-55:~/Desktop/extratask$ git init
Initialized empty Git repository in /home/dci/Desktop/extratask/.git/
dci@dci-Aspire-A515-55:~/Desktop/extratask$ code books.md
dci@dci-Aspire-A515-55:~/Desktop/extratask$ code .
dci@dci-Aspire-A515-55:~/Desktop/extratask$ git add books.md; git add movies.md
dci@dci-Aspire-A515-55:~/Desktop/extratask$ git commit
[master (root-commit) ccb3ff5] I did add 2 files to repository
 2 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 books.md
 create mode 100644 movies.md
dci@dci-Aspire-A515-55:~/Desktop/extratask$ code .
dci@dci-Aspire-A515-55:~/Desktop/extratask$ code .
dci@dci-Aspire-A515-55:~/Desktop/extratask$ git commit
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   books.md
	modified:   movies.md

no changes added to commit (use "git add" and/or "git commit -a")
dci@dci-Aspire-A515-55:~/Desktop/extratask$ git add books.md; git add movies.md
dci@dci-Aspire-A515-55:~/Desktop/extratask$ git commit
[master 7dc40d5] I did make changes in MD files
 2 files changed, 17 insertions(+)
dci@dci-Aspire-A515-55:~/Desktop/extratask$ touch readme.md
dci@dci-Aspire-A515-55:~/Desktop/extratask$ git add readme.md
dci@dci-Aspire-A515-55:~/Desktop/extratask$ code .

dci@dci-Aspire-A515-55:~/Desktop/extratask$ git add readme.md
dci@dci-Aspire-A515-55:~/Desktop/extratask$ git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
	new file:   readme.md

dci@dci-Aspire-A515-55:~/Desktop/extratask$ git log
commit 7dc40d5b540204641c24638db30201e9fd8710b7 (HEAD -> master)
Author: Boruchigor <boruchigor@gmail.com>
Date:   Tue Oct 13 15:27:43 2020 +0200

    I did make changes in MD files

commit ccb3ff51e0a809fe83dcf7f4af8e68eea60248db
Author: Boruchigor <boruchigor@gmail.com>
Date:   Tue Oct 13 15:16:28 2020 +0200

    I did add 2 files to repository
dci@dci-Aspire-A515-55:~/Desktop/extratask$ 


ci@dci-Aspire-A515-55:~/Desktop/extratask$ code .
dci@dci-Aspire-A515-55:~/Desktop/extratask$ git add readme.md
dci@dci-Aspire-A515-55:~/Desktop/extratask$ git commit
[master f166127] changes to readme.md
 1 file changed, 56 insertions(+)
 create mode 100644 readme.md
dci@dci-Aspire-A515-55:~/Desktop/extratask$ git checkout -b Fixmovies
Switched to a new branch 'Fixmovies'
dci@dci-Aspire-A515-55:~/Desktop/extratask$ git checkout
dci@dci-Aspire-A515-55:~/Desktop/extratask$ git branch
* Fixmovies
  master
dci@dci-Aspire-A515-55:~/Desktop/extratask$ code .
dci@dci-Aspire-A515-55:~/Desktop/extratask$ 
dci@dci-Aspire-A515-55:~/Desktop/extratask$ git branch master
fatal: A branch named 'master' already exists.
dci@dci-Aspire-A515-55:~/Desktop/extratask$ git checkout master
#Switched to branch 'master'
dci@dci-Aspire-A515-55:~/Desktop/extratask$ git branch
  Fixmovies
* master
dci@dci-Aspire-A515-55:~/Desktop/extratask$ code .
dci@dci-Aspire-A515-55:~/Desktop/extratask$ git merge Fixmovies
Updating f166127..c5febb5
Fast-forward
 books.md  |  1 +
 movies.md |  7 ++++++-
 readme.md | 16 ++++++++++++++++
 3 files changed, 23 insertions(+), 1 deletion(-)
dci@dci-Aspire-A515-55:~/Desktop/extratask$ git commit
On branch master
nothing to commit, working tree clean
dci@dci-Aspire-A515-55:~/Desktop/extratask$ code .
dci@dci-Aspire-A515-55:~/Desktop/extratask$ touch otherbooks.md
dci@dci-Aspire-A515-55:~/Desktop/extratask$ code .
dci@dci-Aspire-A515-55:~/Desktop/extratask$ git add otherbooks.md
dci@dci-Aspire-A515-55:~/Desktop/extratask$ git log
commit c5febb5ab74b58f117efe64e9bf063fb874a21fa (HEAD -> master, Fixmovies)
Author: Boruchigor <boruchigor@gmail.com>
Date:   Tue Oct 13 15:45:51 2020 +0200

    changes to all files

commit f166127ba84cedffb936c4d6b0715104f3ae948d
Author: Boruchigor <boruchigor@gmail.com>
Date:   Tue Oct 13 15:31:32 2020 +0200

    changes to readme.md

commit 7dc40d5b540204641c24638db30201e9fd8710b7
Author: Boruchigor <boruchigor@gmail.com>
Date:   Tue Oct 13 15:27:43 2020 +0200

    I did make changes in MD files

commit ccb3ff51e0a809fe83dcf7f4af8e68eea60248db
Author: Boruchigor <boruchigor@gmail.com>
Date:   Tue Oct 13 15:16:28 2020 +0200

    I did add 2 files to repository
dci@dci-Aspire-A515-55:~/Desktop/extratask$ git commit
[master 4c1689a] added otherbooks
 1 file changed, 9 insertions(+)
 create mode 100644 otherbooks.md
dci@dci-Aspire-A515-55:~/Desktop/extratask$ git log
commit 4c1689acbbc15c64981af67bef73bcba11f808a9 (HEAD -> master)
Author: Boruchigor <boruchigor@gmail.com>
Date:   Tue Oct 13 15:48:28 2020 +0200

    added otherbooks

commit c5febb5ab74b58f117efe64e9bf063fb874a21fa (Fixmovies)
Author: Boruchigor <boruchigor@gmail.com>
Date:   Tue Oct 13 15:45:51 2020 +0200

    changes to all files

commit f166127ba84cedffb936c4d6b0715104f3ae948d
Author: Boruchigor <boruchigor@gmail.com>
Date:   Tue Oct 13 15:31:32 2020 +0200

    changes to readme.md

commit 7dc40d5b540204641c24638db30201e9fd8710b7
Author: Boruchigor <boruchigor@gmail.com>
Date:   Tue Oct 13 15:27:43 2020 +0200

    I did make changes in MD files

commit ccb3ff51e0a809fe83dcf7f4af8e68eea60248db
Author: Boruchigor <boruchigor@gmail.com>
Date:   Tue Oct 13 15:16:28 2020 +0200

    I did add 2 files to repository
dci@dci-Aspire-A515-55:~/Desktop/extratask$ 

