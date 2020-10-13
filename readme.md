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
