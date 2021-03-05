# Docker_Grafana

Le but est de pouvoir mettre en place deux conteneurs (mysql et grafana) sur un serveur à distance accessible via une adresse IP.

## Installation des logiciels nécessaires

On aura besoin des logiciels suivant:
- [Docker desktop pour windows](https://www.docker.com/products/docker-desktop) pour gérer nos diffirénts conteneurs
![image](/Images/Graphana.png)
- [Filezila](https://filezilla-project.org/) qui nous permettra de pouvoir déposer des fichiers directement sur le serveur où l'on souhaite déployer nos conteneurs
![image](/Images/Filezila.png)

## Manipulation à faire

Les différents fichiers dont on aura besoin sont les suivants:

- [vaccination.sql](/vaccination.sql) qui contient les données qui seront insérées dans le volume de notre conteneur mysql. Si l'on souhaite changer de base données ou en créer  une autre (en rapport avec celle(s) présentes dans notre conteneur mysql), il faudra modifier les lignes 22 et 30.
![image](/Images/vaccination.png) 
- [docker-compose.yml](/docker-compose.yml): qui va se charger de builder nos différents conteneurs (mysql et grafana) avec les différents paramètres (à savoir le nom des différents conteneurs les volumes à mettre à en place, les mots de passe si besoin,les autorisations à donner pour grafana [admin ou viewer] etc).
![image](/Images/Docker-compose.png)
- [automatic.yml](/datasources/automatic.yml) qui contient les différents paramètres de configuration de la datasource de grafana 
![image](/Images/automatic.png)
- [dashoard.yml](/dashbords/dashboard.yml) qui définti les paramètres de nos dashboards
![image](/Images/dashboard-config.png)
- les différents fichiers json:[graphana.json](/dashboards/grafana.json),[test-1614937473893.json](/dashboards/test-1614937473893.json),[vdsdsc-1614943367241.json](/dashboards/vdsdsc-1614943367241.json)( qui sont en fait les différents dashboard contenant les différents graphes)


