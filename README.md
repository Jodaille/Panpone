# Panpone
Ceech Arduino pour barrière protectrice des ruches contre Vespa Velutina

## Présentation de la carte Astri Arista

https://www.openhardware.io/view/44/Solar-powered-sensor-board

https://www.tindie.com/products/ceech/astri-arista/

### La petite soeur d'Arduino

À base de contrôleur Atmega 328p comme le Arduino Pro mini,
il fonctionne en 3,3V à 8 MHz.

Une fréquence de 8 MHz implique une tension de travail de 3,3V, contre 5V et
16 MHz pour Arduino Uno ou Nano, cela permet d'obtenir une consommation
électrique plus faible et par conséquent une autonomie plus importante.

### Gestion de la charge de la batterie MPPT avec LTC4079

Accepte les batteries Li-Ion/Polymer, acide-plomb ou NiMH batterie, jusqu'à 60V.

La charge maximale est définie via une résistance avec 100 Ma max.,
sans règlage le voltage est de 4,2V.

## Programmation de la carte via le port série

### Liaison série
La carte est dépourvue de controlleur série.

Elle dispose de connecteurs permettant de relier un controlleur série de type
FTDI.

Les connecteurs sont nommés:

RS
TX
RX
3V3
GND
GND

### Éditeur Arduino

Il peut être obtenu sur le site d'Arduino :

Dans la section : Download the Arduino IDE
https://www.arduino.cc/en/Main/Software

### Paramètrage du port série

En fonction de l'adaptateur, du système d'exploitation, le port série peut-être
nommé différement. Il arrive aussi qu'après un mauvais contact, le port utilisé
change, par exemple sous Linux avec un adaptateur FTDI, il peut passer facilement
de /dev/ttyUSB0 à /dev/ttyUSB1 et inversement.

Dans l'IDE Arduino, menu
Choisir carte Arduino Micro/Pro mini, 3,3V @ 8mHz
