# TD GIT

### Consultation de l'état : 
Vérifiez l'état actuel de votre dépôt avec la commande status.
```
[dorian@laptop cours_git]$ git status
On branch section-5-6
nothing to commit, working tree clean
[dorian@laptop cours_git]$
```

Pour vérifier les changements apporté dans les anciens commit avec git log

```
[dorian@laptop cours_git]$ git log
commit 93dec547902fd512b9dde00239866a5f27bfbd4c (HEAD -> section-5-6, origin/section-5-6)
Author: Dorian Cruveiller <doriancruveiller@gmail.com>
Date:   Thu Jan 18 17:06:48 2024 +0100

    Add 2 sections

commit ef8078d9421a21ceaa6175179e58fd960de8d9f1 (origin/cours_git, origin/HEAD, cours_git)
Author: Dorian Cruveiller <doriancruveiller@gmail.com>
Date:   Thu Jan 18 16:56:47 2024 +0100

    Add README.md

commit 1c03fa7f02c32f3812f9648c833b093ee49953fa
Author: Dusséaux Thomas <t.dusseaux@gmail.com>
Date:   Thu Jan 18 16:52:54 2024 +0100

    maj

commit 9a36f5143690db2e473d3f78812175a00ed37ea4
Author: Dusséaux Thomas <t.dusseaux@gmail.com>
Date:   Thu Jan 18 14:42:44 2024 +0100

[dorian@laptop cours_git]$
```

### Mise à jour du dépôt local :
Récupérez les dernières modifications depuis le dépôt distant.
```
git pull origin nom_de_la_branche
```

Ex:
```
[dorian@laptop cours_git]$ git pull origin cours_git
From https://github.com/Detzio/cours_git
 * branch            cours_git  -> FETCH_HEAD
Already up to date.
[dorian@laptop cours_git]$
```
### Initialisation d'un nouveau dépôt :
Pour démarrer un nouveau projet, il faut initialiser un dépôt Git dans le répertoire de votre projet.
```
cd chemin/vers/votre/projet # Se rendre dans le répertoire souhaité
git init # Initialisation du dossier git
```

### Clonage d'un dépôt existant :
Pour copier l'état actuel d'un dépôt distant en local
```
git clone url_du_depot
```
### Envoi des modifications au dépôt distant
Après avoir validé les modifications, il faut les envoyer au dépôt distant avec la commande `git push` pour les envoyer dans la branche courante ou `git push origin <nom_branche>` pour envoyer dans une branche spécifique.

### Création d'une branche
Pour créer une branche, afin de travailler sur une fonctionnalité spécifique par exemple, il faut utiliser la commande `git checkout -b <nom_branche>`.

### Fusion des branches : 
Fusionner une branche dans une autre après avoir terminé le travail.
```
git checkout branche_cible
```

```
git merge branche_source
```

### Historique des commits : 
Consulter l'historique des commits avec la commande log.
```
git log
```

Consulter les modifications par rapport à ce commit
```
git show
```