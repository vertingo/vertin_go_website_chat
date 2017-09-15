# Socket.io : Chat

Cette application reprend les sources du tutoriel présent sur le blog [bini.io](http://blog.bini.io) :

* [Partie 1](http://blog.bini.io/developper-une-application-avec-socket-io/)
* [Partie 2](http://blog.bini.io/developper-un-chat-avec-socket-io-partie-2/)
* [Partie 3](http://blog.bini.io/developper-un-chat-avec-socket-io-partie-3/)

Ce tutoriel est lui même une adaptation du [tutoriel officiel](http://socket.io/get-started/chat/) de socket.io.

Cette version ajoute les fonctionnalités suivantes par rapport à la version du tutoriel officiel :

* Support des noms d'utilisateurs
* Affichage d'un message lors de la connexion/déconnexion d'un utilisateur
* Affichage de la liste des utilisateurs connectés
* Conservation d'un historique des messages
* Affichage du texte "typing" à côté du nom des utilisateurs en train de saisir un message


## Installation

Si vous n'avez pas bower d'installé sur votre machine, installez-le au préalable de la façon suivante :
Egalement si vous n'avez pas Node.Js afin d'éxécuter les commandes npm téléchargez le sur l'url suivant: https://nodejs.org/en/
```
Une fois installé placer dans le dossier racine du chat en loccurence: socket.io-chat-master et éxécuter les commandes ci-dessous dans une invite de commande((Clic droit + Shift ==> Ouvrir une invite de comande!))!
npm install -g bower
```
Pour installer l'application, téléchargez les sources (zip ou git clone) et exécutez la commande suivante depuis la racine du projet.
```
npm install
bower install
```

## Démarrer l'application localement

Pour démarrer l'application, exécutez la commande suivante depuis la racine du projet.
```
node server
```
L'application est désormais accesssible à l'url **http://localhost:3000/**.

## Déployer votre application via Git sur EvenNode.com(https://admin.evennode.com/login?continue=http%3A%2F%2Fadmin.evennode.com%2Fa%2Flist)
Si vous n'avez pas de compte git creer votre compte à l'url suivant:  https://github.com/business?utm_source=google&utm_medium=cpc&utm_term=git&utm_campaign=2018q1-adv-EMEA|NB|Git|FR|EN|EX|20160906
Télécharger et installer également git localement afin de pouvoir éxécuter les commandes ci-dessous! ==> https://git-scm.com/download/win

Ensuite éxécuter les commandes ci-dessous dans le répertoire de votre projet via une invite de commande(Clic droit + Shift ==> Ouvrir une invite de comande!) pour instancier un dépot local git:

```
git init
git add .
git commit -m "first commit"
git remote add origin https://github.com/[Git_Name_Account]/[Git_Project_Name].git
git push -u origin master
```
Si vous rencontrez ce genre d'erreur: fatal: refusing to merge unrelated histories
Executez la commande ci-dessous: git pull origin branchname --allow-unrelated-histories

Une fois votre projet upload dans votre dépot git connecter vous à EvenNode(https://admin.evennode.com/login?continue=http%3A%2F%2Fadmin.evennode.com%2Fa%2Flist) 
et créer votre compte EvenNode gratuitement pour déployer votre application sur le web!
Ensuite créer une nouvelle application en cliquant sur le bouton create new app!

- Télécharger maintenant putty: https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html
- Cliquer sur le bouton generate!
- Bouger votre souris au-dessus de PuttyGen jusqu'à ce que votre clé soit généré!
- Cliquer sur le menu Conversion -> Export OpenSSH key
- Sauvegardé votre clé privé dans le répertoire suivant: C:\Users\your_username\.ssh\id_rsa
- Copié votre clé public dans votre compte EvenNode dans le menu manage Puclic Key

Retourner dans votre dossier racine de votre projet et éxécuter les ligne de commande suivante:

Pour cette commande vous devez remplacer la partie your_app_here par votre clé de répertoire git sur votre compte EvenNode 
soit par exemple la partie entre crochet(N'incluez pas les crochet) de l'exemple suivant: git@git.evennode.com:[b3d71189e8e580bb1944b02145721033.git]

```
git remote add evennode git@git.evennode.com:your_app_here
git push evennode master
```
A ce stade là il est probable qu'il manque le dossier components dans le sous répertoire public/
Dans ce cas taper les commandes suivantes pour le rajouter dans git puis push de nouveau le répertoire EvenNode:

```
cd public
git add -f components
git commit -m "second commit"
git push -u origin master
git push evennode master
```

Et voilà normalement votre application est désormais en ligne sur votre compte EvenNode!

```
Un petit coup de pouce suivez nous sur YouTube et Facebook!
[You Tube] ==> https://www.youtube.com/channel/UC2g_-ipVjit6ZlACPWG4JvA?sub_confirmation=1
[Facebook] ==> https://www.facebook.com/vertingo/
```
<p align="center">
  <a href="https://www.youtube.com/channel/UC2g_-ipVjit6ZlACPWG4JvA?sub_confirmation=1"><img src="http://vertin-go.com/Fonctions_Annexes/annexes/pdt-page-de-telechargement/Android%20You%20Tube%20Data%20API/youtube2.png" width="400" height="250"/></a>
  <a href="https://www.facebook.com/vertingo/"><img src="http://vertin-go.com/Fonctions_Annexes/annexes/pdt-page-de-telechargement/Android%20You%20Tube%20Data%20API/rejoins_nous.png" width="400" height="250"/></a>
</p>



