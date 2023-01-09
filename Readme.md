# Exercice n°1 : 

[comment]: <> (ceci me pertmet d'ecrire un commentaire)

Vous allez créer un projet sur votre dépot git.

Vous allez appeler votre projet “exercice1”

***solution :***
>*Se rendre sur [Github](https://github.com) ou [Gitlab](https://about.gitlab.com/) est creer un nouveau repository (public) avec le nom exercice1*

## Ci-dessous les étapes à effectuer :

● En local, vous allez créer un projet qui sera composé d’un fichier texte, qui s'appellera “fichier1” dans lequel vous saisir le texte suivant :
○ Je suis l'exercice 1 de “votre prénom".

***solution :***
>*Creer un nouveau dossier exerice1 sur son poste est démarrer un dépot git local* commande possible :
```
mkdir exercice1
cd exercice1
git init
echo " Je suis l'exercice 1 de 'Anne Onyme'. " >> fichier1.txt
```



● Il faudra faire en sorte que ce fichier soit présent sur votre dépôt distant sur git dans votre projet “exercice1”.

***solution :***
> Premiére étape ajouter ce fichier à notre dépot local et le commit :
```
git add fichier1.txt
git commit -m "création de fichier1.txt avec le message Je suis l'exercice 1 de 'votre prénom'."
```
> Deuxiéme étape ajouter l'adresse de notre dépot distant (github) a notre dépot local :
```
git remote add origin https://github.com/nom_utilisateur_github/exercice1.git
git branch -M main
```
> Derniére étape mettre à jour notre dépot distant
```
git push -u origin main
```



● une fois que cela aura été fait, il faudra créer un nouveau fichier texte que l’on va appeler “fichier2”.
● Ce nouveau fichier devra contenir le texte suivant :
○ Je suis l'exercice 1 mais je suis le second fichier

***solution :***
>Creer un fichier exerice2 :
```
echo "Je suis l'exercice 1 mais je suis le second fichier" >> fichier2.txt
git add fichier2.txt
git commit -m "création de fichier2.txt avec le message Je suis l'exercice 1 mais je suis le second fichier"
```

● Ce fichier qui s’appelle fichier2 sera lui aussi pousser sur votre dépôt distant au sein de votre projet “exercice1”.

***solution :***
>Mise à jour de notre dépot distant :
```
git push -u origin main
```