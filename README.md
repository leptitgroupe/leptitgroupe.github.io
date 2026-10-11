# Site du P'tit Groupe

Le site du P'tit Groupe est un site statique généré en utilisant l'outil *Jekyll*

## Setup linux

Ce qu'il est nécessaire d'installer pour commencer

```bash
sudo apt install ruby-bundler
sudo apt install ruby-dev build-essential
sudo gem install jekyll
sudo apt install rbenv
rbenv install 3.0.0
eval "$(rbenv init -)"
bundle update --bundler
bundle install
```
## Setup windows
 
TBD

## Génération du site en local

Dans le dossier du site, lancer

```bash
bundle exec jekyll serve
```

Le site est généré à l'addresse locale http://127.0.0.1:4000/

## Mettre à jour le site

Le site est constitué de pages html ou markdown qui vont chercher des information dans des fichiers de configuration yaml.

* [Page principale](index.md)
* [Contact](_data/contact.yml)
* [Prochains concerts](_data/gigs.yml)
* [Enregistrements](_data/recordings.yml)

Pour ajouter un concert passé dans [Souvenir de concerts](http://127.0.0.1:4000/live.html)

Créé un nouveau fichier dans [_posts](_posts) en prenant example sur un post existant (exemple [concert au five oh](_posts/2024-08-22-foveoh.md)) et ajouter les photos dans [assets/images/posts/](assets/images/posts/)

Les changements sont visible directement sur le site local, et seront appliqués sur le vrai site après les avoir poussés sur github.
Il est recommandé de d'abord vérifier les changements en local pour ne pas risquer de casser le site.