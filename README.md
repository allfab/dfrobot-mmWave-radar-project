# Détection de présence à ondes millimétriques : DFRobot mmWave Radar Project
ESPHome - mmWave Presence Detection - Home Assistant - DFRobot - Wemos D1 Mini - Node Red
 
Ce projet s'inspire de la vidéo de **Everything Smart Home** et de sa vidéo **["I Built My Own Presence Detection Sensor!"](https://www.youtube.com/watch?v=VEqWlOeJ2YA)**

L'un des projets les plus utiles déployés à ce jour à l'aide d'Home Assistant est l'éclairage basé sur le mouvement.
Le but du projet est de créer un détecteur de présence à ondes millimétriques basé sur un Wemos D1 Mini et un capteur à ondes millimétriques 24 GHz (mmWW) permettant de détecter une présence jusqu'à 9 m. Ce module communique avec un microcontrôleur compatible Arduino via une interface UART.

Le détecteur de présence ainsi construit sera ensuite couplé à Home Assisatnt via ESPHome et un flux Node Red pour l'automation. 

Le capteur retenu est le capteur de la marque DFRobot SEN0395 qui a les fonctionnalités suivantes :
+ Détection de la présence humaine : détecter s'il y a un corps humain dans les zones,
+ Forte capacité anti-interférence : n'est pas affecté par la neige, la brume, la température, l'humidité, la poussière, la lumière, le bruit, etc...



### Liens
+ mmWave sensor (DFRobot) : https://www.gotronic.fr/art-detecteur-de-presence-mmwave-sen0395-34207.htm
+ Wemos D1 Mini : https://www.amazon.fr/dp/B08BTRPMV1?ref_=cm_sw_r_cp_ud_dp_PRTYDE7ZZDD44NCW4G22
+ Forum Home Assistant : https://bit.ly/3agi5YE
+ DFRobot Wiki Page : https://bit.ly/3wZ3Jn1