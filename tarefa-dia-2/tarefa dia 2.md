
sylvia.albuquerque@TD-432 MINGW64 ~
$ git config --global user.name "Sylvia Albuquerque"

sylvia.albuquerque@TD-432 MINGW64 ~
$ git config --global user.email sylvia_albuquerque@hotmail.com

sylvia.albuquerque@TD-432 MINGW64 ~
$ git config --list
diff.astextplain.textconv=astextplain
filter.lfs.clean=git-lfs clean -- %f
filter.lfs.smudge=git-lfs smudge -- %f
filter.lfs.process=git-lfs filter-process
filter.lfs.required=true
http.sslbackend=openssl
http.sslcainfo=C:/Program Files/Git/mingw64/ssl/certs/ca-bundle.crt
core.autocrlf=true
core.fscache=true
core.symlinks=false
pull.rebase=false
credential.helper=manager-core
credential.https://dev.azure.com.usehttppath=true
init.defaultbranch=master
user.name=Sylvia Albuquerque
user.email=sylvia_albuquerque@hotmail.com

sylvia.albuquerque@TD-432 MINGW64 ~
$ cd desktop

sylvia.albuquerque@TD-432 MINGW64 ~/desktop
$ git clone https://github.com/SylviaAlbuquerque/aprenda-a-programar.git
Cloning into 'aprenda-a-programar'...
warning: You appear to have cloned an empty repository.

sylvia.albuquerque@TD-432 MINGW64 ~/desktop
$ git status
fatal: not a git repository (or any of the parent directories): .git

sylvia.albuquerque@TD-432 MINGW64 ~/desktop
$ cd aprenda-a-programar

sylvia.albuquerque@TD-432 MINGW64 ~/desktop/aprenda-a-programar (master)
$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        tarefa-dia-1/

nothing added to commit but untracked files present (use "git add" to track)

sylvia.albuquerque@TD-432 MINGW64 ~/desktop/aprenda-a-programar (master)
$ git add .

sylvia.albuquerque@TD-432 MINGW64 ~/desktop/aprenda-a-programar (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   tarefa-dia-1/resum0-dia-1.md


sylvia.albuquerque@TD-432 MINGW64 ~/desktop/aprenda-a-programar (master)
$ git commit -m "subindo documento"
[master (root-commit) 8748b9b] subindo documento
 1 file changed, 98 insertions(+)
 create mode 100644 tarefa-dia-1/resum0-dia-1.md

sylvia.albuquerque@TD-432 MINGW64 ~/desktop/aprenda-a-programar (master)
$ git log
commit 8748b9b0786796885fac126e0120d393ebc3d8f5 (HEAD -> master)
Author: Sylvia Albuquerque <sylvia_albuquerque@hotmail.com>
Date:   Wed Aug 24 08:22:36 2022 -0300

    subindo documento

sylvia.albuquerque@TD-432 MINGW64 ~/desktop/aprenda-a-programar (master)
$ q
bash: q: command not found

sylvia.albuquerque@TD-432 MINGW64 ~/desktop/aprenda-a-programar (master)
$ mkdir tarefa-dia-2

sylvia.albuquerque@TD-432 MINGW64 ~/desktop/aprenda-a-programar (master)
$ lls
bash: lls: command not found

sylvia.albuquerque@TD-432 MINGW64 ~/desktop/aprenda-a-programar (master)
$ ls
tarefa-dia-1/  tarefa-dia-2/

sylvia.albuquerque@TD-432 MINGW64 ~/desktop/aprenda-a-programar (master)
$ cd tarefa-dia-2

sylvia.albuquerque@TD-432 MINGW64 ~/desktop/aprenda-a-programar/tarefa-dia-2 (master)
$ touch index.html

sylvia.albuquerque@TD-432 MINGW64 ~/desktop/aprenda-a-programar/tarefa-dia-2 (master)
$ ls
index.html

sylvia.albuquerque@TD-432 MINGW64 ~/desktop/aprenda-a-programar/tarefa-dia-2 (master)
$ git status
On branch master
Your branch is based on 'origin/master', but the upstream is gone.
  (use "git branch --unset-upstream" to fixup)

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        ./

nothing added to commit but untracked files present (use "git add" to track)

sylvia.albuquerque@TD-432 MINGW64 ~/desktop/aprenda-a-programar/tarefa-dia-2 (master)
$ cd ..

sylvia.albuquerque@TD-432 MINGW64 ~/desktop/aprenda-a-programar (master)
$ git status
On branch master
Your branch is based on 'origin/master', but the upstream is gone.
  (use "git branch --unset-upstream" to fixup)

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        tarefa-dia-2/

nothing added to commit but untracked files present (use "git add" to track)

sylvia.albuquerque@TD-432 MINGW64 ~/desktop/aprenda-a-programar (master)
$ git add
Nothing specified, nothing added.
hint: Maybe you wanted to say 'git add .'?
hint: Turn this message off by running
hint: "git config advice.addEmptyPathspec false"

sylvia.albuquerque@TD-432 MINGW64 ~/desktop/aprenda-a-programar (master)
$ git add .

sylvia.albuquerque@TD-432 MINGW64 ~/desktop/aprenda-a-programar (master)
$ git status
On branch master
Your branch is based on 'origin/master', but the upstream is gone.
  (use "git branch --unset-upstream" to fixup)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   tarefa-dia-2/index.html


sylvia.albuquerque@TD-432 MINGW64 ~/desktop/aprenda-a-programar (master)
$ git commit -m "subindo index"
[master dc35d9d] subindo index
 1 file changed, 11 insertions(+)
 create mode 100644 tarefa-dia-2/index.html

sylvia.albuquerque@TD-432 MINGW64 ~/desktop/aprenda-a-programar (master)
$ git push
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 8 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (8/8), 1.58 KiB | 537.00 KiB/s, done.
Total 8 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/SylviaAlbuquerque/aprenda-a-programar.git
 * [new branch]      master -> master

sylvia.albuquerque@TD-432 MINGW64 ~/desktop/aprenda-a-programar (master)
$ cd tarefa-dia-2

sylvia.albuquerque@TD-432 MINGW64 ~/desktop/aprenda-a-programar/tarefa-dia-2 (master)
$ touch pratica-1.js

sylvia.albuquerque@TD-432 MINGW64 ~/desktop/aprenda-a-programar/tarefa-dia-2 (master)
$ touch pratica-2.js

sylvia.albuquerque@TD-432 MINGW64 ~/desktop/aprenda-a-programar/tarefa-dia-2 (master)
$ touch pratica-3.js

sylvia.albuquerque@TD-432 MINGW64 ~/desktop/aprenda-a-programar/tarefa-dia-2 (master)
$ touch pratica-4.js

sylvia.albuquerque@TD-432 MINGW64 ~/desktop/aprenda-a-programar/tarefa-dia-2 (master)
$ ls
index.html  pratica-1.js  pratica-2.js  pratica-3.js  pratica-4.js

sylvia.albuquerque@TD-432 MINGW64 ~/desktop/aprenda-a-programar/tarefa-dia-2 (master)
$ cd..
bash: cd..: command not found

sylvia.albuquerque@TD-432 MINGW64 ~/desktop/aprenda-a-programar/tarefa-dia-2 (master)
$ cd aprenda-a-programar
bash: cd: aprenda-a-programar: No such file or directory

sylvia.albuquerque@TD-432 MINGW64 ~/desktop/aprenda-a-programar/tarefa-dia-2 (master)
$ cd..
bash: cd..: command not found

sylvia.albuquerque@TD-432 MINGW64 ~/desktop/aprenda-a-programar/tarefa-dia-2 (master)
$ cd desktop
bash: cd: desktop: No such file or directory

sylvia.albuquerque@TD-432 MINGW64 ~/desktop/aprenda-a-programar/tarefa-dia-2 (master)
$ cd

sylvia.albuquerque@TD-432 MINGW64 ~
$ cd desktop

sylvia.albuquerque@TD-432 MINGW64 ~/desktop
$ cd aprenda-a-programar

sylvia.albuquerque@TD-432 MINGW64 ~/desktop/aprenda-a-programar (master)
$ git status
On branch master
Your branch is up to date with 'origin/master'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        tarefa-dia-2/pratica-1.js
        tarefa-dia-2/pratica-2.js
        tarefa-dia-2/pratica-3.js
        tarefa-dia-2/pratica-4.js

nothing added to commit but untracked files present (use "git add" to track)

sylvia.albuquerque@TD-432 MINGW64 ~/desktop/aprenda-a-programar (master)
$ git add .

sylvia.albuquerque@TD-432 MINGW64 ~/desktop/aprenda-a-programar (master)
$ git commit -m "subindo arquivos pratica"
[master 4755cc3] subindo arquivos pratica
 4 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 tarefa-dia-2/pratica-1.js
 create mode 100644 tarefa-dia-2/pratica-2.js
 create mode 100644 tarefa-dia-2/pratica-3.js
 create mode 100644 tarefa-dia-2/pratica-4.js

sylvia.albuquerque@TD-432 MINGW64 ~/desktop/aprenda-a-programar (master)
$ git log
commit 4755cc34803b2c5f17eaa9154d9610fa19ad2060 (HEAD -> master)
Author: Sylvia Albuquerque <sylvia_albuquerque@hotmail.com>
Date:   Wed Aug 24 08:46:42 2022 -0300

    subindo arquivos pratica

commit dc35d9d1346ba229aee01c96f2173b8f74446397 (origin/master)
Author: Sylvia Albuquerque <sylvia_albuquerque@hotmail.com>
Date:   Wed Aug 24 08:32:10 2022 -0300

    subindo index

commit 8748b9b0786796885fac126e0120d393ebc3d8f5
Author: Sylvia Albuquerque <sylvia_albuquerque@hotmail.com>
Date:   Wed Aug 24 08:22:36 2022 -0300

    subindo documento

sylvia.albuquerque@TD-432 MINGW64 ~/desktop/aprenda-a-programar (master)
$ git push
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (4/4), 385 bytes | 192.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/SylviaAlbuquerque/aprenda-a-programar.git
   dc35d9d..4755cc3  master -> master

sylvia.albuquerque@TD-432 MINGW64 ~/desktop/aprenda-a-programar (master)
$ cd tarefa-dia-2

sylvia.albuquerque@TD-432 MINGW64 ~/desktop/aprenda-a-programar/tarefa-dia-2 (master)
$ node pratica-1.js
bash: node: command not found

sylvia.albuquerque@TD-432 MINGW64 ~/desktop/aprenda-a-programar/tarefa-dia-2 (master)
