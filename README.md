# Préambule

Slides du cours disponibles [ici](http://slides.com/women_on_rails/week-1)

Ce tutoriel a pour objectif de mettre en place un environnement de travail propre pour commencer un nouveau projet Ruby On Rails dans le cadre du cycle 1 des ateliers Women On Rails.

# Étape 1 : Notions utiles

Voici une liste de commandes que vous allez utiliser dans ce tutoriel. Certaines concernent des notions qui seront abordées dans les ateliers suivants du cycle.

## Commandes principales de la console

La console permet d'interagir avec votre machine sans utiliser d'interface graphique (qui est plus limitée et moins rapide d'utilisation). Vous pouvez par exemple créer un nouveau fichier ou vous déplacer dans des dossiers en utilisant les commandes suivantes:

- cd : Permet de se déplacer à travers les répertoires (+ tab pour autocompletion). Exemple: ``` cd images ```
- ls : Liste les fichiers et dossiers de votre répertoire courrant. Exemple: ``` ls ```
- touch : Permet de créer des fichiers. Exemple: ``` touch index.html ```
- mkdir : Permet de créer des répertoires. Exemple: ``` mkdir stylesheets ```
- cp : Permet de copier un fichier ou un répertoire. Exemple: ``` cp images ```
- mv : Permet de déplacer un fichier ou un répertoire. Exemple: ``` mv custom.css stylesheets/ ```
- pwd : Permet de savoir dans quel répertoire on est. Exemple ``` pwd ```
- rm : Permet de détruire un élément sur la machine. Exemple: ``` rm index.html ``` détruit le fichier ``` index.html ```

## Commandes principales de Git

Git est un outil permettant de travailler en équipe et de versionner son travail.

Voici les commandes principales que nous allons utiliser tout au long du projet, pour utiliser Git:

- git init : Utile pour tout nouveau projet. Cela permet d'initialiser git dans le dossier de travail.
- git clone : Crée une copie du projet distant (ce que vous voyez sur github par exemple) sur votre orginateur (en local).
- git status : Permet de voir les différences entre ce que vous avez en ce moment dans les fichiers et ce que git a compris "depuis la dernière sauvegarde". Exemple: ``` git status ```
- git add : Ajoute un changement aux modifications à prendre en compte (à l'index). Exemples: ``` git add -p ``` pour choisir l'ajout fichier par fichier, ```git add . ``` pour tout ajouter
- ```git commit -m "Mon message"``` : Permet d'enregistrer de manière permanente en y associant un message.
- ```git push origin master``` : Envoie toutes les modifications enregistrées vers le répertoire distant (vers Github dans notre cas)

Voir [ce lien](http://rogerdudler.github.io/git-guide/index.fr.html) pour plus d'informations.

## Commandes Ruby On Rails

- ```rails new curiosites``` : Crée un nouveau projet RubyOnRails avec ```curiosites``` comme nom de projet
- ```rails new .``` : Crée un nouveau projet RubyObRails dans le dossier courrant
- ```rails server``` : (ou ```rails s```) Lance un serveur local permettant de tester l'application sur son ordinateur avec l'aide d'un navigateur

# Étape 2 : Démarrage du projet Curiosités

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

#### Création du compte Cloud9

[Cloud9](https://c9.io/signup) propose la création de comptes gratuits.

![Creation Compte Cloud9](/images/readme/cloud9_creation_compte.png)

#### Création du workspace

Après la création de votre compte, vous aurez la possibilité de créer un nouveau workspace (espace de travail).

![Votre compte](/images/readme/cloud9_creation_workspace.png)

Cliquez sur ``` Create a new workspace ```.

![Workspace Cloud9](/images/readme/lien_cloud9_github.png)

Renseignez le nom de votre projet (``` curiosites ``` par exemple), le lien vers Github, le modèle Ruby (section ```Template```) et cliquez sur le bouton de création.

#### Difficultés possibles

Si à cette étape vous rencontrez une erreur (problème de clé SSH), vous allez avoir besoin d'identifier votre compte Could9 auprès de votre compte Github de manière sécurisée.

Plus d'infos sur les clés SSH [ici](http://sebsauvage.net/comprendre/ssl/).

Rendez vous sur votre compte Github et allez sur votre profil.

![Recherche Profil](/images/readme/recherche_profil.png)

Puis cliquez sur ``` Edit profile ``` pour aller sur la page de configuration de votre compte.

Suite à cela, choisissez le menu ``` SSH and GPG keys ```.

![Acces configuration SSH](/images/readme/settings.png)

Cette section va vous permettre d'ajouter une nouvelle clé SSH relative à votre compte Cloud9. La clé SSH se trouve sur votre compte [Cloud9](https://c9.io/) et est accessible dans les paramètres.

![Parametres Cloud9](/images/readme/parametres_cloud9.png)

Dans la section ``` SSH Keys ```, copiez la clé SSH qui vous est indiquée.

![Ou trouver la clé SSH Cloud9](/images/readme/copie_cle_ssh.png)

Retournez sur votre compte [Github](https://github.com/settings/keys) et ajoutez la clé précedemment copié dans votre presse-papier.

![Créer une nouvelle clé SSH](/images/readme/creation_cle_ssh.png)

Voila ! Retournez sur Cloud9 pour essayer de nouveau la création d'un nouveau workspace.

#### Utilisation de l'espace de travail

Vous arrivez sur un éditeur de texte intégré dans votre navigateur:

![Cloud9 Editeur](/images/readme/workspace_vide.png)

Utilisez le terminal pour créer une application Ruby On Rails et construire automatiquement les fichiers de base de votre projet avec la commande ``` rails new . ```

![Rails New](/images/readme/rails_new.png)

Cela va générer de nouveaux fichiers dans votre projet.
![Projet rempli](/images/readme/projet_rempli.png)

Lancez un serveur Rails avec le bouton ``` Run Project ``` dans votre workspace Cloud9 pour pouvoir visualiser la page d'accueil de votre application. L'url à utiliser dans le navigateur sera indiquée dans le terminal.

Bravo ! Vous venez de tester avec succès l'environnement sur lequel vous travaillerez tout au long du cycle.

# Étape 3 : Enregistrer les modifications sur le répertoire distant

[Enregistrer vos modifications et les envoyer sur votre répertoire Github](https://women-on-rails.github.io/guide/push_project)

# Liens Utiles :
- Commencer avec GIT : http://christopheducamp.com/2013/12/15/github-pour-nuls-partie-1/ ou http://rogerdudler.github.io/git-guide/index.fr.html
- Aller plus loin avec les répertoires distants : https://git-scm.com/book/fr/v1/Les-bases-de-Git-Travailler-avec-des-d%C3%A9p%C3%B4ts-distants
- Premiers pas en CSS : http://css.mammouthland.net/premiers-pas-en-css.php
- Principales balises en HTML : https://openclassrooms.com/courses/apprenez-a-creer-votre-site-web-avec-html5-et-css3/memento-des-balises-html ou http://www.vieytes.org/tbalises.html
- Guide complet sur le HTML : http://www.lehtml.com/html/index.htm
- Les clés SSH : http://sebsauvage.net/comprendre/ssl/