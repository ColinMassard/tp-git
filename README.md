# Javascript

- `npm install` &rarr; installation des dépendances
- `npm run lint` &rarr; vérifie de bon formattage du code
- `npm run format` &rarr; formate de code
- `npm run test` &rarr; lance les tests unitaires



## Partie 1 - Explications (14 points)

Cette partie est une restitution des connaissances que vous avez acquises sur l'utilisation de Git et Github. Plutôt que de vous laisser libre sur la rédaction, cela est sous forme de questions-réponses. Détaillez en utilisant les concepts vus en cours (zones, cycle de vie, référence...).
Pour répondre aux questions, créez une nouvelle branche et créez une Merge Request afin que je puisse faire une revue simplement.

### Quelle sont les deux façons d'initialiser un dépôt ? (1 point)
Pour initialiser un dépôt git deux options sont possible :
D'un côté cloné un projet avec git clone à partir d'un remote controller.
De l'autre initialiser le projet et crée le remote controller depuis son environnement avec la commande git init cette dernière ajoutant un fichier .git créeant un dossier sur le remote controller avec la branche master correspondante

### À quoi sert une Pull Request / Merge Request ? (1 point)
Une pull request ou merge request est une demande venant d'un autre utilisateur pour fusionné les modifications qu'il à apporté à votre référentiel.

### Qu'est ce qu'une branche ? (1 point)
Une Branche est pointeur de commit

### Vous venez de modifier un fichier. Comment créer un commit ? (3 points)
Premièrement avec git add nom-du-fichier on ajoute tous le fichiers au commit que l'on va crée
Avec git commit -m "Notre message" on crée notre commit avec un nom personnalisé en fonction de nos modifications
Enfin on envoie nos modifications sur le remote controller avec git push

### Pourquoi est-il plus prudent d'utiliser `origin/master` plutôt que `master` pour se mettre à jour ? (1 point)
Master cible le master local sur lequel on pourrait travailler avec notre ordinateur tandis que origin/master cible le master du remote controller et donc le plus a même d'être le plus à jour.

### A quoi servent les commandes `git status`, `git log` et `git reflog` ? Quand les utiliser ? (2 points)
Git Status : Affiche le status de la branche actuelle ( Fichier modifié / Ajouté au commit )
Git Log: Montre les logs des commits
Git reflog : gère les info de reflog en espace de référence
En les utilisant on peut voir le status actuel de notre version


### Quelles sont les conditions qui doivent être réunies pour que des conflits surviennent ? (2 points)
Deux personnes travaillent sur la même branche et push.
Lors d'un merge lors qu'on essaye d'intégrer des modifications à un fichier


### Imaginez que la branche master du dépôt distant contient de nouveaux commits. Comment intégrer ces commits dans votre branche ? (3 points)
Git fetch -all
Git rebase master
