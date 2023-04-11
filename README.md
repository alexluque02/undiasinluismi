# undiasinluismi

He clonado el repositorio en local y hago el commit inicial
git add .
touch .gitignore
touch privado.txt
mkdir privada
code .

privado.txt
privada/ Escribo esto en .gitgnore

git add .
git commit -m "Añadiendo archivos ignorados por git"
touch fichero1.txt
git tag -a v0.1 -m "Version 0.1."
push

git checkout -b "v.02"
touch 2.txt
add .
commit 
git push --all


Alex Luque@DESKTOP-IBH7I11 MINGW64 ~/undiasinluismi (v.02)
$ git checkout main
Switched to branch 'main'
M       README.md
M       fichero1.txt
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

Alex Luque@DESKTOP-IBH7I11 MINGW64 ~/undiasinluismi (main)
$ code .

Alex Luque@DESKTOP-IBH7I11 MINGW64 ~/undiasinluismi (main)
$ git commit -am "Escribo Hola"
[main bab2aa9] Escribo Hola
 2 files changed, 7 insertions(+)

Alex Luque@DESKTOP-IBH7I11 MINGW64 ~/undiasinluismi (main)
$ git checkout v.02
Switched to branch 'v.02'

Alex Luque@DESKTOP-IBH7I11 MINGW64 ~/undiasinluismi (v.02)
$ code .

Alex Luque@DESKTOP-IBH7I11 MINGW64 ~/undiasinluismi (v.02)
$ git commit -am "Escribo Adiós"
[v.02 ad5a56d] Escribo Adiós
 1 file changed, 1 insertion(+)

Alex Luque@DESKTOP-IBH7I11 MINGW64 ~/undiasinluismi (v.02)
$ git checkout main
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 2 commits.
  (use "git push" to publish your local commits)

Alex Luque@DESKTOP-IBH7I11 MINGW64 ~/undiasinluismi (main)
$ git merge v.02
Auto-merging fichero1.txt
CONFLICT (content): Merge conflict in fichero1.txt
Automatic merge failed; fix conflicts and then commit the result.

Alex Luque@DESKTOP-IBH7I11 MINGW64 ~/undiasinluismi (main|MERGING)
$ code .

Alex Luque@DESKTOP-IBH7I11 MINGW64 ~/undiasinluismi (main|MERGING)
$ git branch --merged
* main

Alex Luque@DESKTOP-IBH7I11 MINGW64 ~/undiasinluismi (main|MERGING)
$ git branch --no-merged
  v.02

Alex Luque@DESKTOP-IBH7I11 MINGW64 ~/undiasinluismi (main|MERGING)
$ git add .

Alex Luque@DESKTOP-IBH7I11 MINGW64 ~/undiasinluismi (main|MERGING)
$ git commit -am "Resolvemos conflicto"
[main ce4ab7b] Resolvemos conflicto

Alex Luque@DESKTOP-IBH7I11 MINGW64 ~/undiasinluismi (main)
$ git tag -a v0.2 -m "Version 0.2"

Alex Luque@DESKTOP-IBH7I11 MINGW64 ~/undiasinluismi ((ad5a56d...))
$ git checkout main
Previous HEAD position was ad5a56d Escribo Adiós
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 4 commits.
  (use "git push" to publish your local commits)

Alex Luque@DESKTOP-IBH7I11 MINGW64 ~/undiasinluismi (main)
$ git branch
* main
  v.02

Alex Luque@DESKTOP-IBH7I11 MINGW64 ~/undiasinluismi (main)
$ git branch -d v.02
Deleted branch v.02 (was ad5a56d).


