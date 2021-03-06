# Détection de présence à ondes millimétriques : DFRobot mmWave Radar Project
ESPHome - mmWave Presence Detection - Home Assistant - DFRobot - Wemos D1 Mini - Node Red

![DFRobot mmWave Radar SEN0395](https://raw.githubusercontent.com/allfab/dfrobot-mmWave-radar-project/main/02-DFRobot%20mmWave%20SEN0395/Images/ori-detecteur-de-presence-mmwave-sen0395-34207-light.jpg)
![AZDelivery D1 Mini V3](https://raw.githubusercontent.com/allfab/dfrobot-mmWave-radar-project/main/01-Arduino%20D1%20Mini%20V3/Images/d1miniv3-light.jpg)


Ce projet s'inspire de la vidéo de **Everything Smart Home** et de sa vidéo **["I Built My Own Presence Detection Sensor!"](https://www.youtube.com/watch?v=VEqWlOeJ2YA)**

L'un des projets les plus utiles déployés à ce jour à l'aide d'Home Assistant est l'éclairage basé sur le mouvement.
Le but du projet est de créer un détecteur de présence à ondes millimétriques basé sur un Wemos D1 Mini et un capteur à ondes millimétriques 24 GHz (mmWW) permettant de détecter une présence jusqu'à 9 m. Ce module communique avec un microcontrôleur compatible Arduino via une interface UART.

Le détecteur de présence ainsi construit sera ensuite couplé à Home Assisatnt via ESPHome et un flux Node Red pour l'automation. 

Le capteur retenu est le capteur de la marque DFRobot SEN0395 qui a les fonctionnalités suivantes :
+ Détection de la présence humaine : détecter s'il y a un corps humain dans les zones,
+ Forte capacité anti-interférence : n'est pas affecté par la neige, la brume, la température, l'humidité, la poussière, la lumière, le bruit, etc...


### Diagramme de connexion

##### D1 Mini V3 <-> DFRobot mmWave SEN0395

![Diagramme](https://raw.githubusercontent.com/allfab/dfrobot-mmWave-radar-project/main/03-Connection%20diagram/Connection%20Diagram%20-%20D1%20Mini%20V3%20-%20DFRobot%20mmWave%20Radar.png)

| D1 Mini V3    | DFRobot mmWave SEN0395 |
|:-------------:|:----------------------:|
| D1            | Rx                     |
| D2            | Tx                     |
| D0 (GPIO16)   | IO2                    |
| V 5v          | V                      |
| G             | G                      |

##### D1 Mini V3 - Brochage
![Brochage D1 Mini V3](https://raw.githubusercontent.com/allfab/dfrobot-mmWave-radar-project/main/01-Arduino%20D1%20Mini%20V3/Images/D1-Mini-V3-pinout-light.png)


### Liens
+ mmWave sensor (DFRobot) : https://www.gotronic.fr/art-detecteur-de-presence-mmwave-sen0395-34207.htm
+ Wemos D1 Mini : https://www.amazon.fr/dp/B08BTRPMV1?ref_=cm_sw_r_cp_ud_dp_PRTYDE7ZZDD44NCW4G22
+ Forum Home Assistant : https://community.home-assistant.io/t/mmwave-presence-detection-esphome-style/382778
+ DFRobot Wiki Page : https://wiki.dfrobot.com/mmWave_Radar_Human_Presence_Detection_SKU_SEN0395
