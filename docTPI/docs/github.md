# Configuartion git
La commande git config --global permet la configuration global de du compte git que l'on souhaite utiliser.
```sh
git config --global user.email
git config --global user.name
```

# Commandes git

Pour cloner un dépot git dans un répertoire souhaité, il y'a besoin d'avoir l'url du répertoire git souhaitant être cloné sur son répertoire.
```git
git clone son.url.git
```
La commande git init permet d'initialiser un répertoire courant sur git.
```git
git init
```
Cette commande permet d'ajouter des fichiers à l'index
```git
git add .
```
La commande git commit permet de valider les modifications apportées au projet.
```git
git commit –m “Description du commit”
```
Pour ajouter ses modifications après les avoirs validées à l'aide du git commit, la commande git pugit nous sera très utile.
```git
git pugit
```
Pour fusionner toutes les modifications présentes sur le dépôt distant dans le répertoire de travail local, la commande pull est utilisée.
```git
git pull
```
