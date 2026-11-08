## Comandes de Git

### Crear i clonar repositoris

| Comanda                                   | Descripció                                                         |
| ----------------------------------------- | ------------------------------------------------------------------ |
| `git init`                                | Inicialitza un repositori local de Git                             |
| `git clone ssh://git@github.com/[nom-usuari]/[nom-repo].git` | Crea una còpia local d'un repositori remot      |

### Comandes bàsiques

| Comanda                                 | Descripció                                                        |
| --------------------------------------- | ----------------------------------------------------------------- |
| `git status`                            | Comprova l'estat actual                                           |
| `git add [nom-arxiu.txt]`               | Afegeix un fitxer a la zona de pujar canvis                       |
| `git add -A`                            | Afegeix tots els fitxers del repositori a la zona de pujar canvis |
| `git commit -m "[missatge]"`            | Crea un missatge explicatiu dels canvis                           |
| `git rm -r [nom-arxiu.txt]`             | Elimina un fitxer (o carpeta)                                     |

### Branques i fusions

| Comanda                   | Descripció                                                                                             |
| ------------------------- | ------------------------------------------------------------------------------------------------------ |
| `git branch`              | Mostra una llista de les branques que hi ha (l'asterisc assenyala la branca activa)                    |
| `git branch -a`           | Mostra una llista de totes les branques (locals i remotes)                                             |
| `git branch [nom]`        | Crea una nova branca                                                                                   |
| `git branch -d [nom]`     | Elimina una branca local                                                                               |
| `git push origin --delete [nom]`      | Elimina una branca remota                                                                  |
| `git checkout -b [nom]`               | Crea una nova branca i ens posicionem                                                      |
| `git checkout -b [nom] origin/[nom]`  | Clona una branca remota i ens posicionem ahí                                               |
| `git branch -m [nom-antic] [nom-nou]` | Renomena una branca local                                                                  |
| `git checkout [nom-branca]`           | Canvia a una branca concreta                                                               |
| `git checkout -`                      | Canvia a la última branca activa                                                           |
| `git checkout -- [nom-arxiu]`         | Descarta canvis en un fitxer                                                               |
| `git merge [nom-branca]`              | Combina una branca amb la branca activa                                                    |
| `git merge [nom-branca-origen] [nom-branca-desti]` | Combina una branca (branca-origen) amb una branca nova (branca-desti)         |
| `git stash`                           | Reverteix els darrers canvis i errors en el directori actual                               |
| `git stash clear`                     | Reverteix tots els canvis en el directori actual                                           |

### Compartir i actualitzar projectes

| Comanda                                       | Descripció                                                                     |
| --------------------------------------------- | ------------------------------------------------------------------------------ |
| `git push origin [nom-branca]`                | Envia una branca local al repositori remot                                     |
| `git push -u origin [nom-branca]`             | Envia canvis al repositori remot (i et posiciona a la branca concreta)         |
| `git push`                                    | Envia canvis al repositori remot (en la branca actual)                         |
| `git push origin --delete [nom-branca]`       | Elimina una branca remota                                                      |
| `git pull`                                    | Actualitza el repositori local a l'últim commit fet                            |
| `git pull origin [nom-branca]`                | Porta / agafa tots els canvis d'un dipòsit remot                               |
| `git remote add origin ssh://git@github.com/[nom-usuari]/[nom-repo].git` | Afegeix canvis a un repositori remot                |
| `git remote set-url origin ssh://git@github.com/[nom-usuari]/[nom-repo].git` | Ubica la branca remota d'un repositori remot mitjançant SSH |

### Inspeccionar i comparar

| Comanda                                    | Descripció                                     |
| ------------------------------------------ | ---------------------------------------------- |
| `git log`                                  | Visualitza els canvis                          |
| `git log --summary`                        | Visualitza els canvis (en detall)              |
| `git log --oneline`                        | Visualitza els canvis (resumit)                |
| `git diff [branca-origen] [branca-desti]`  | Vista prèvia dels canvis abans de fer un merge |
