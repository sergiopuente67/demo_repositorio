﻿# demo_repositorio

puent@JoseVicente MINGW64 ~ (master)
$ git config --global user.name "Sergio"
git config --global user.email "sergio.puente@alumnos.uneatlantico.es"

puent@JoseVicente MINGW64 ~ (master)
$

puent@JoseVicente MINGW64 ~ (master)
$ git clone <https://github.com/sergiopuente67/demo_repo.git>
bash: syntax error near unexpected token `newline'

puent@JoseVicente MINGW64 ~ (master)
$ git clone https://github.com/sergiopuente67/demo_repositorio.git
Cloning into 'demo_repositorio'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 3 (delta 0), pack-reused 0 (from 0)
Receiving objects: 100% (3/3), done.

puent@JoseVicente MINGW64 ~ (master)
$ cd demo_repositorio

puent@JoseVicente MINGW64 ~/demo_repositorio (main)
$ ^[[200~mkdir origen destino
bash: $'\E[200~mkdir': command not found

puent@JoseVicente MINGW64 ~/demo_repositorio (main)
$ mkdir origen destino

puent@JoseVicente MINGW64 ~/demo_repositorio (main)
$ git add .

puent@JoseVicente MINGW64 ~/demo_repositorio (main)
$ git commit -m "Crear carpetas origen y destino"
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

puent@JoseVicente MINGW64 ~/demo_repositorio (main)
$ git commit -m "Crear carpetas origen y destino"
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

puent@JoseVicente MINGW64 ~/demo_repositorio (main)
$ ^[[200~echo "Este es un texto aleatorio" > origen/archivo1.txt
bash: $'\E[200~echo': command not found

puent@JoseVicente MINGW64 ~/demo_repositorio (main)
$ echo "Este es un texto aleatorio" > origen/archivo1.txt
echo "Otro texto aleatorio" > origen/archivo2.txt

puent@JoseVicente MINGW64 ~/demo_repositorio (main)
$ git add origen
warning: in the working copy of 'origen/archivo1.txt', LF will be replaced by CRLF the next time Git touches it
warning: in the working copy of 'origen/archivo2.txt', LF will be replaced by CRLF the next time Git touches it

puent@JoseVicente MINGW64 ~/demo_repositorio (main)
$ git commit -m "Crear archivos con texto aleatorio en la carpeta origen"
[main e72e0a6] Crear archivos con texto aleatorio en la carpeta origen
 2 files changed, 2 insertions(+)
 create mode 100644 origen/archivo1.txt
 create mode 100644 origen/archivo2.txt

puent@JoseVicente MINGW64 ~/demo_repositorio (main)
$ echo "Texto modificado en el archivo 1" > origen/archivo1.txt
echo "Texto modificado en el archivo 2" > origen/archivo2.txt

puent@JoseVicente MINGW64 ~/demo_repositorio (main)
$ git add origen
warning: in the working copy of 'origen/archivo1.txt', LF will be replaced by CRLF the next time Git touches it
warning: in the working copy of 'origen/archivo2.txt', LF will be replaced by CRLF the next time Git touches it

puent@JoseVicente MINGW64 ~/demo_repositorio (main)
$ git commit -m "Modificar los textos de los archivos en origen"
[main 4b2eac5] Modificar los textos de los archivos en origen
 2 files changed, 2 insertions(+), 2 deletions(-)

puent@JoseVicente MINGW64 ~/demo_repositorio (main)
$ mv origen/* destino/

puent@JoseVicente MINGW64 ~/demo_repositorio (main)
$ git add .
warning: in the working copy of 'destino/archivo1.txt', LF will be replaced by CRLF the next time Git touches it
warning: in the working copy of 'destino/archivo2.txt', LF will be replaced by CRLF the next time Git touches it

puent@JoseVicente MINGW64 ~/demo_repositorio (main)
$ git commit -m "Mover archivos de origen a destino"
[main 99f76b1] Mover archivos de origen a destino
 2 files changed, 0 insertions(+), 0 deletions(-)
 rename {origen => destino}/archivo1.txt (100%)
 rename {origen => destino}/archivo2.txt (100%)

puent@JoseVicente MINGW64 ~/demo_repositorio (main)
$ echo "Texto nuevamente modificado en el archivo 1" > destino/archivo1.txt
echo "Texto nuevamente modificado en el archivo 2"
Texto nuevamente modificado en el archivo 2

puent@JoseVicente MINGW64 ~/demo_repositorio (main)
$
   git add destino
warning: in the working copy of 'destino/archivo1.txt', LF will be replaced by CRLF the next time Git touches it

puent@JoseVicente MINGW64 ~/demo_repositorio (main)
$ git commit -m "Modificar textos de los archivos en destino"
[main f58e717] Modificar textos de los archivos en destino
 1 file changed, 1 insertion(+), 1 deletion(-)

puent@JoseVicente MINGW64 ~/demo_repositorio (main)
$ git push origin main
Enumerating objects: 17, done.
Counting objects: 100% (17/17), done.
Delta compression using up to 4 threads
Compressing objects: 100% (11/11), done.
Writing objects: 100% (16/16), 1.50 KiB | 384.00 KiB/s, done.
Total 16 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/sergiopuente67/demo_repositorio.git
   174c744..f58e717  main -> main

puent@JoseVicente MINGW64 ~/demo_repositorio (main)
