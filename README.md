# Hackathon Frioul ![CI status](http://myprovence.code4marseille.fr/media/logo/code4marseille.png)

Code4Marseille est une association composée de 3 écoles de formation en web developpement : Le Wagon, Webforce3 et Simplon.

L'objectif du Hackaton est de montrer la force de ces 3 formations a coder ensemble un projet en peu de temps. Ce projet, a destination des touristes désirant découvrir la magnifique région de Marseille et de ces environs, a une dimension temps réel et une dimension de partage entre utilisateurs non négligeable.

## Requirements
* Apache
* MySql
* Php > 7.1.3
* Composer 1.7.2
* Git

## Installation des outils

Selon votre système installez Mamp ou Wamp (vrsion 64bits) et pensez à sélectionner une version de PHP > à 7.1.3

Installez composer soit directement sur votre machine windows en installant l’exécutable soit en utilisant le fichier composer.phar à la racine de votre projet. 
Voir le site [Composer](https://getcomposer.org/download/)

Installez la prise en charge de Git en ligne de commande [GIT](https://git-scm.com/downloads)


## Installation du Front

* Installez WAMP ou LAMP sur votre machine. 
* Dans le répertoire du serveur Web local, créez un répertoire pour le projet front
* Cloner le dépôt distant avec git clone `$ https://github.com/nienfba/hackathon_front.git`
* Vous êtes prêt à utilisez le Front, connectez vous à votre dossier à partir de localhost (ex : http://localhost/hackthon_front)

## Installation du Back

* Installez WAMP ou LAMP sur votre machine
* Dans le répertoire du serveur Web local, créez un répertoire pour le projet front
* Cloner le dépôt distant avec git clone `$ https://github.com/nienfba/hackathon_back.git`
* Configurez votre php.ini en modifiant la valeur memory_limit. Affectez la valeur -1 (mamory_limit=-1)

### Installez Symfony et ses dépendances

* utilisez composer en ligne de commande
`$ composer update` ou `$php composer.phar update`
* une fois le framework et ses dépendances mises à jour, modifier le fichier .env à la racine. Trouvez le ligne `$ DATABASE_URL=mysql://db_user:db_password@127.0.0.1:3306/db_name` 
Remplacez db_user et db_password par vos valeur locales. Pour une installation standard de Wamp : 
`$ DATABASE_URL=mysql://root:@127.0.0.1:3306/db_name` 

Serveur Web Machine WAMP ou MAMP (pas de XAMP !): attention PHP > 7.1.3
    Modifier le php.ini > memory_limit = -1 pour installation Symfony par la suite

Installer Composer
    PC : 
    MAC : 

Git en ligne de commande

Détails sur les 2 dépots Git

Récupération du Front dans un dossier front_hackathon
    Le front est fonctionnel. L'ensemble des données du Front sont pour le moment récupérées sur le site http://myprovence.code4marseille.fr/api/
    Pour vos développement nous vous demandons d'effectuer vos requêtes ajax 

Récupération du Back dans un dossier back_hackathon
    Installation du Back
    
    >> Composer update (attention php doit utiliser un max de mémoire memory_limit = -1 dans php.ini de php 7.2)

    Modification du fichier .env pour modifier le mot de passe vers la base de données
    Création de la base symfony create_database
    Création des tables symfony make:migration
    Création du contenu symfony doctrine:fixtures:load

    On a maintenant des utilisateurs et du contenu dans la base
    Pour le moment il n'est pas nécessaire d'accéder à l'administration du Back, il est fonctionnel pour votre projet en Front

    Le Back fourni une API pour LIRE, et ECRIRE des données. Elle est documentée, vous pouvez 

    Il est disponible ici http://localhost/back_hackathon/api/

    Pour chaque fonctionnalité de l'API vous pouvez accéder aux détails






    



### Requirements
* Apache
* MySql
* Php > 7.1.3

`$ pip install foobar`

## Installation

### Requirements
* Visual Studio, Sublime Text ou Atom
* Terminal



## Usage

```python
import foobar

foobar.pluralize('word') # returns 'words'
foobar.pluralize('goose') # returns 'geese'
foobar.singularize('phenomena') # returns 'phenomenon'
```

## Development
```
$ virtualenv foobar
$ . foobar/bin/activate
$ pip install -e .
```

## Contributing

Comment travailler à plusieurs sur un même projet.

Taper cette ligne de commande dans le terminal :

mkdir ~/code/OWNER_GITHUB_USERNAME
cd ~/code/OWNER_GITHUB_USERNAME
git clone git@github.com:OWNER_GITHUB_USERNAME/PROJECT_NAME.git
cd PROJECT_NAME

ATTENTION, il faut copier coller la clef SSH donnée par l'invitation !


Vous voila en COLLABORATION :)

Dans le but de ne pas perdre le travail de chacun il est OBLIGATOIRE de travailler sur une branche afin de ne pas écraser le travail de chacun

Pour cela le terminal est votre ami :

git branch -b nom-de-votre-branche 
( le nom doit être le plus explicatif possible afin de pouvoir comprendre ce qui est a l'intérieur de la branche et ce même 5 mois après par un inconnu )

Pour voir votre travail sur le master il faut pusher votre branche par cette ligne de commande :

git push origin nom-de-votre-branche

Il faut ensuite créer une pull request sur GitHub afin de savoir si il y a des conflits entre vos travails respectifs sur le repo.

La validation de cette pull request la push automatiquement sur le master.

Il vous suffit ensuite de faire un git PULL origin master afin de récupérer le master à jour


VOUS VOILA FIN PRETS POUR DU BON TRAVAIL DE GROUPE.

