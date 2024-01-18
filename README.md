# TD GIT

### Consultation de l'état : 
Vérifiez l'état actuel de votre dépôt avec la commande status.
```
[dorian@laptop cours_git]$ git status
On branch section-5-6
nothing to commit, working tree clean
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