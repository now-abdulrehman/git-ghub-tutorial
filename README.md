
usera@NOW MINGW64 ~/Documents/1-MyCode/Git/git-ghub-tutorial
$ git --version
git version 2.55.0.windows.5

usera@NOW MINGW64 ~/Documents/1-MyCode/Git/git-ghub-tutorial
$ git init
Initialized empty Git repository in C:/Users/usera/Documents/1-MyCode/Git/git-ghub-tutorial/.git/

usera@NOW MINGW64 ~/Documents/1-MyCode/Git/git-ghub-tutorial (main)
$ git status
On branch main

No commits yet

nothing to commit (create/copy files and use "git add" to track)

usera@NOW MINGW64 ~/Documents/1-MyCode/Git/git-ghub-tutorial (main)
$ git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        index.html

nothing added to commit but untracked files present (use "git add" to track)

usera@NOW MINGW64 ~/Documents/1-MyCode/Git/git-ghub-tutorial (main)
$ git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        index.html
        script.js
        style.css

nothing added to commit but untracked files present (use "git add" to track)

usera@NOW MINGW64 ~/Documents/1-MyCode/Git/git-ghub-tutorial (main)
$ git add index.html

usera@NOW MINGW64 ~/Documents/1-MyCode/Git/git-ghub-tutorial (main)
$ git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   index.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        script.js
        style.css


usera@NOW MINGW64 ~/Documents/1-MyCode/Git/git-ghub-tutorial (main)
$ git commit -m "Add index.html
> "git status
error: pathspec 'status' did not match any file(s) known to git

usera@NOW MINGW64 ~/Documents/1-MyCode/Git/git-ghub-tutorial (main)
$ git git add style.css script.js
git: 'git' is not a git command. See 'git --help'.

The most similar command is
        init

usera@NOW MINGW64 ~/Documents/1-MyCode/Git/git-ghub-tutorial (main)
$ git add style.css script.js

usera@NOW MINGW64 ~/Documents/1-MyCode/Git/git-ghub-tutorial (main)
$ git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   index.html
        new file:   script.js
        new file:   style.css


usera@NOW MINGW64 ~/Documents/1-MyCode/Git/git-ghub-tutorial (main)
$ git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   index.html
        new file:   script.js
        new file:   style.css


usera@NOW MINGW64 ~/Documents/1-MyCode/Git/git-ghub-tutorial (main)
$ git rm --cached index.html style.css script.js
rm 'index.html'
rm 'script.js'
rm 'style.css'

usera@NOW MINGW64 ~/Documents/1-MyCode/Git/git-ghub-tutorial (main)
$ git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        index.html
        script.js
        style.css

nothing added to commit but untracked files present (use "git add" to track)

usera@NOW MINGW64 ~/Documents/1-MyCode/Git/git-ghub-tutorial (main)
$ git add index.html

usera@NOW MINGW64 ~/Documents/1-MyCode/Git/git-ghub-tutorial (main)
$ git commit -m "Add index.html"
[main (root-commit) 4c28e56] Add index.html
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 index.html

usera@NOW MINGW64 ~/Documents/1-MyCode/Git/git-ghub-tutorial (main)
$ git add style.css script.js

usera@NOW MINGW64 ~/Documents/1-MyCode/Git/git-ghub-tutorial (main)
$ git commit -m "Add style.css & script.js"
[main 444630e] Add style.css & script.js
 2 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 script.js
 create mode 100644 style.css

usera@NOW MINGW64 ~/Documents/1-MyCode/Git/git-ghub-tutorial (main)
$ git status
On branch main
nothing to commit, working tree clean

usera@NOW MINGW64 ~/Documents/1-MyCode/Git/git-ghub-tutorial (main)
$ git log
commit 444630e2d84a28c0b80370c7c4b3e421e0c461b6 (HEAD -> main)
Author: Abdul Rehman <userar28@gmail.com>
Date:   Fri Sep 4 19:38:40 2026 +0500

    Add style.css & script.js

commit 4c28e56373fe8782b99ba23fa966fe6c6ecba8c0
Author: Abdul Rehman <userar28@gmail.com>
Date:   Fri Sep 4 19:37:01 2026 +0500

    Add index.html

usera@NOW MINGW64 ~/Documents/1-MyCode/Git/git-ghub-tutorial (main)
$ git log --oneline
444630e (HEAD -> main) Add style.css & script.js
4c28e56 Add index.html

usera@NOW MINGW64 ~/Documents/1-MyCode/Git/git-ghub-tutorial (main)
$ git status
On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   index.html

no changes added to commit (use "git add" and/or "git commit -a")

usera@NOW MINGW64 ~/Documents/1-MyCode/Git/git-ghub-tutorial (main)
$ git restore --staged index.html

usera@NOW MINGW64 ~/Documents/1-MyCode/Git/git-ghub-tutorial (main)
$ git status
On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   index.html

no changes added to commit (use "git add" and/or "git commit -a")

usera@NOW MINGW64 ~/Documents/1-MyCode/Git/git-ghub-tutorial (main)
$ git add index.html

usera@NOW MINGW64 ~/Documents/1-MyCode/Git/git-ghub-tutorial (main)
$ git status
On branch main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   index.html


usera@NOW MINGW64 ~/Documents/1-MyCode/Git/git-ghub-tutorial (main)
$ git add index.html

usera@NOW MINGW64 ~/Documents/1-MyCode/Git/git-ghub-tutorial (main)
$ git commit -m "Add main heading"
[main 89bf2f9] Add main heading
 1 file changed, 1 insertion(+)

usera@NOW MINGW64 ~/Documents/1-MyCode/Git/git-ghub-tutorial (main)
$ git status
On branch main
nothing to commit, working tree clean

usera@NOW MINGW64 ~/Documents/1-MyCode/Git/git-ghub-tutorial (main)
$ git log
commit 89bf2f999745b6ff242644be04b5f2784e9a1d3a (HEAD -> main)
Author: Abdul Rehman <userar28@gmail.com>
Date:   Fri Sep 4 20:06:27 2026 +0500

    Add main heading

commit 444630e2d84a28c0b80370c7c4b3e421e0c461b6
Author: Abdul Rehman <userar28@gmail.com>
Date:   Fri Sep 4 19:38:40 2026 +0500

    Add style.css & script.js

commit 4c28e56373fe8782b99ba23fa966fe6c6ecba8c0
Author: Abdul Rehman <userar28@gmail.com>
Date:   Fri Sep 4 19:37:01 2026 +0500

    Add index.html

usera@NOW MINGW64 ~/Documents/1-MyCode/Git/git-ghub-tutorial (main)
$ git log --oneline
89bf2f9 (HEAD -> main) Add main heading
444630e Add style.css & script.js
4c28e56 Add index.html

usera@NOW MINGW64 ~/Documents/1-MyCode/Git/git-ghub-tutorial (main)
$ git log --oneline
89bf2f9 (HEAD -> main) Add main heading
444630e Add style.css & script.js
4c28e56 Add index.html

usera@NOW MINGW64 ~/Documents/1-MyCode/Git/git-ghub-tutorial (main)
$
