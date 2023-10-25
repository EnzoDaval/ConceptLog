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


## Grafana

- Installer Grafana : https://grafana.com/docs/grafana/latest/setup-grafana/installation/


## MIT App Inventor

- Se créer un compte sur MIT App Inventor
- Connecter son ordinateur et son téléphone à un même réseau Wi-Fi, différent de celui de l'école.
- Télécharger le fichier : Mettre le lien.
- L'import dans MIT App Inventor.
- Dans le bloc "When Clock2.Timer", une adresse est indiqué dans deux blocs "join". Il faut mettre son adresse ip, trouvable en lançant la commande "ipconfig" dans un cmd. [https://github.com/EnzoDaval/ConceptLog/blob/main/screen/screen.png]


## Node Red

- Installer Node-Red : https://nodered.org/docs/getting-started/local
- Télécharger le fichier : Mettre le lien.
- Lancer Node-Red en lançant la commande "node-red" en ligne de commande puis y accéder via l'adresse http://localhost:1880/
- Import le fichier dans Node-Red.
- Sur les noeuds influxDB des différents flux, choisir votre serveur en mettant le token InfluxDB dans le champs "Token". [https://github.com/EnzoDaval/ConceptLog/blob/main/screen/token.png]
- Déployer le projet.
