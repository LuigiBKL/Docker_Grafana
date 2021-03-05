# Docker_Grafana

Le but est de pouvoir mettre en place deux conteneurs (mysql et grafana) sur un serveur à distance accessible via une adresse IP.

## Installation des logiciels nécessaires

On aura besoin des logiciels suivant:
-[Docker desktop pour windows](https://www.docker.com/products/docker-desktop) pour gérer nos diffirénts conteneurs
-[Filezila](https://filezilla-project.org/) qui nous permettra de pouvoir déposer des fichiers directement sur le serveur où l'on souhaite déployer nos conteneurs

## Manipulation à faire

Les différents fichiers dont on aura besoin sont les suivants:

-vaccination.sql qui contient les données qui seront insérer dans le volume de notre conteneur mysql
-docker-compose: qui va se charger de builder nos différents conteneurs (mysql et grafana) avec les différents paramètres (à savoir le nom des différents conteneurs les volumes à mettre à en place, les mots de passe si besoin 



