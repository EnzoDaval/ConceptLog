# Conception Logicielle, smart phone au wearable computer

## Rappel du projet

Projet logiciel de collecte d'informations depuis des terminaux mobiles jusqu'à des services de stockage sur une BDD temporelle dotées d'outils d'analyse


## Membres

- DAVAL Enzo
- TRICOT Thomas
- LORCERY morgane
- BEVAN Tom


## Architecture du projet
![Architecture du projet](https://raw.githubusercontent.com/EnzoDaval/ConceptLog/main/screen/Fonctionnement_Projet.png)


## InfluxDB

- Installer InfluxDB : https://docs.influxdata.com/influxdb/v2/install/
- Noter le token de votre Bucket.
- Y accéder via l'adresse http://localhost:8086/


## Grafana

- Installer Grafana : https://grafana.com/docs/grafana/latest/setup-grafana/installation/
- - Y accéder via l'adresse http://localhost:3000/


## MIT App Inventor

- Se créer un compte sur MIT App Inventor
- Connecter son ordinateur et son téléphone à un même réseau Wi-Fi, différent de celui de l'école.
- Télécharger le fichier : Mettre le lien.
- L'import dans MIT App Inventor.
- Dans le bloc "When Clock2.Timer", une adresse est indiqué dans deux blocs "join". Il faut mettre son adresse ip, trouvable en lançant la commande "ipconfig" dans un cmd. ![MIT App Inventor](https://raw.githubusercontent.com/EnzoDaval/ConceptLog/main/screen/screen.png)


## Node Red

- Installer Node-Red : https://nodered.org/docs/getting-started/local
- Télécharger le fichier : Mettre le lien.
- Lancer Node-Red en lançant la commande "node-red" en ligne de commande puis y accéder via l'adresse http://localhost:1880/
- Import le fichier dans Node-Red.
- Sur les noeuds influxDB des différents flux, choisir votre serveur en mettant le token InfluxDB dans le champs "Token". ![NodeRed](https://raw.githubusercontent.com/EnzoDaval/ConceptLog/main/screen/token.png)
- Déployer le projet.


## Visualisation des graphiques

Les graphiques Grafana sont visualisables sur :
- Sur Grafana.
- Sur l'Interface Utilisateur Node-Red via http://localhost:1880/ui en cliquant sur le menu Burger et en cliquant sur Grafana.

Les graphiques Node-Red sont visualisables sur :
- L'application App Inventor MIT.
- Sur l'Interface Utilisateur Node-Red via http://localhost:1880/ui

## Economie d'énergie 

Optimiser la consommation énergétique implique de minimiser l'utilisation de la bande passante, en évitant une transmission continue des données. Pour cela, on mets en place une stratégie de stockage temporaire sur le téléphone, créant ainsi une petite base de données locale (un cache). De plus, l'intervalle de la clock 2, qui détermine la fréquence à laquelle les données sont transmises, est désactivé au démarrage de l'application, afin de ne pas envoyer de données à ce moment-là.
