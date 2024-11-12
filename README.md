# paysage

$ls || liste les éléments dans le dossier

$cd ini || entre dans le dossier

$mkdir || Créer un dossier 

git add . || ajouter tout les fichiers dans le commit

git commit -m "Message" || commit le fichier ajouté avec message

git push origin || push le fichier ajouté

git branch newImage || crée une branche newImage

git checkout newImage  || focus sur la branche newImage

git merge newImage  || Merge newImage sur la branche ou on se trouve (checkout)

git checkout -b newImage || crée et se focus sur la branche newImage

git rebase main || permet de crée un commit dune copie de la branche sur la branche main. tout en laissant la branche d'origine dispo

HEAD est le commit sur le quel on se trouve actuellement (git checkout c1(hash) pour se positionner sur le commit c1)

git checkout main^ || place HEAD sur le commit qui est le premier parent (main^^ ira au grand parent)

git checkout main ~x || place HEAD sur le commit précedant main de xfois

git branch -f main HEAD~3 || force la branche main de trois commit parents en arrière

git branch -f main C6 || bouge main au commit C6

git reset HEAD~1 || supprime le commit actuel et ramene au précédent

git revert HEAD (placed on C2) || nouveau commit C2' introduit des modifications -- celles qui correspondent justement à l'annulation de celles du commit C2.

git cherry-pick C1 C2 C3 || crée des copies de C1 C2 C3 a la branche on focus

git rebase -i main~4 || permet de copier et replacer main sur 4 parents différents (on peut en ommettre et changer leur position)

git rebase branch main || bouge main sur branch

git commit --amend || commit + une copie

git tag v1 c1 || crée tag V1 en C1

