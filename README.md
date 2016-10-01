# Préambule

Ce tutoriel a pour objectif de mettre en place un environnement de travail propre pour commencer un nouveau projet Ruby On Rails dans le cadre du cycle 1 des ateliers Women On Rails.

# Étape 1 : Notions utiles

Voici une liste de commandes que vous allez utiliser dans ce tutoriel. Certaines concernent des notions qui seront abordées dans les ateliers suivants du cycle.

## Commandes principales de la console

- cd : Permet de se déplacer à travers les répertoires (+ tab pour autocompletion). Exemple: ``` cd images ```
- ls : Liste les fichiers et dossiers de votre répertoire courrant. Exemple: ``` ls ```
- mkdir : Permet de créer des répertoires. Exemple: ``` mkdir stylesheets ```
- cp : Permet de copier un fichier ou un répertoire. Exemple: ``` cp images ```
- mv : Permet de déplacer un fichier ou un répertoire. Exemple: ``` mv custom.css stylesheets/ ```
- pwd : Permet de savoir dans quel répertoire on est. Exemple ``` pwd ```

## Commandes principales de Git

- git status
- git commit
- git add / git add -p
- git branch

## Commandes Ruby On Rails

- ```rails new curiosites``` : Crée un nouveau projet RubyOnRails avec ```curiosites``` comme nom de projet
- ```rails new .``` : Crée un nouveau projet RubyObRails dans le dossier courrant
- ```rails server``` : (ou ```rails s```) Lance un serveur local permettant de tester l'application sur son ordinateur avec l'aide d'un navigateur

# Démarrage du projet Curiosités

## Github

Pour partager vos avancées avec vos mentors, travailler en équipe et ne rien perdre de vos projets, nous conseillons de créer un compte [Github](https://github.com/join?source=header-home).

![Création de compte](/images/readme/github_creation.png)

Lorsque cette étape est finie, vous pourrez créer un nouveau répertoire de travail, sur Github, appelé curiosites.

![Compte Github](/images/readme/github_creation_repertoire.png)

![Création du répertoire de travail](/images/readme/nommage_repertoire.png)

Votre répertoire créé sera vide et pret à etre utilisé.

![Répertoire de travail vide](/images/readme/repertoire_cree.png)

## Installation de l'environnement de travail

Lorsque l'on commence un projet avec Ruby On Rails, certains outils sont pré-requis. On peut soit les installer directement sur une machine, soit utiliser un environnement de travail déjà préparé (Cloud9 ou machines virtuelles).

Si vous débutez dans le monde du développement, nous vous conseillons d'utiliser un environnement déjà préparé pour vous éviter une installation un peu complexe.

### Installation native

[En construction]

### Avec Cloud9

[Cloud9](https://c9.io/signup) propose la création de comptes gratuits.

![Creation Compte Cloud9](/images/readme/cloud9_creation_compte.png)

Après la création de votre compte, vous aurez la possibilité de créer un nouveau workspace (espace de travail).

![Votre compte](/images/readme/cloud9_creation_workspace.png)

Cliquez sur ``` Create a new workspace ```.

![Workspace Cloud9](/images/readme/lien_cloud9_github.png)

Renseignez le nom de votre projet (``` curiosites ``` par exemple), le lien vers Github, le modèle Ruby (section ```Template```) et cliquez sur le bouton de création.

Vous arrivez sur un éditeur de texte intégré dans votre navigateur:

![Cloud9 Editeur](/images/readme/workspace_vide.png)

Utilisez le terminal pour créer une application Ruby On Rails et construire automatiquement les fichiers de base de votre projet avec la commande ``` rails new . ```

![Rails New](/images/readme/rails_new.png)

Cela va générer de nouveaux fichiers dans votre projet.

![Projet rempli](/images/readme/projet_rempli.png)

# Étape 3 : Enregistrer les modifications sur le répertoire distant

[Enregistrer vos modifications et les envoyer sur votre répertoire Github](https://women-on-rails.github.io/guide/push_project)


# Pour aller plus loin :
- Commencer avec GIT : http://christopheducamp.com/2013/12/15/github-pour-nuls-partie-1/
- Aller plus loin avec les répertoires distants : https://git-scm.com/book/fr/v1/Les-bases-de-Git-Travailler-avec-des-d%C3%A9p%C3%B4ts-distants
- Premiers pas en CSS : http://css.mammouthland.net/premiers-pas-en-css.php
- Principales balises en HTML : https://openclassrooms.com/courses/apprenez-a-creer-votre-site-web-avec-html5-et-css3/memento-des-balises-html ou http://www.vieytes.org/tbalises.html
- Guide complet sur le HTML : http://www.lehtml.com/html/index.htm