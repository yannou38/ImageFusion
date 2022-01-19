# ImageFusion

Projet de fusion d'images thermique et visible.

## Pré-requis
- Raspberry pi sous raspian
- S'assurer de la présence du paquet raspistill
- Dans raspiconfig : (**sudo raspi-config**)
  - activer l'ic2 ?
  - donner au moins 124 Mo de mémoire video
- Respecter les branchement des pins GPIO. Les codes des pins nécessaires écrit sur le capteur thermique, ils correspondent aux pins 1,3,5,7,9 sur la raspberry

![GPIO](./gpio.png?raw=true)

- Module pi caméra branché. Dans notre cas il s'agissait de la version 1.3.

## Installation
- Cloner le projet sur la raspberry
- exécuter la commande **make all** qui doit produire un exécutable nommée **thermalCam**

## Utilisation
- exécuter **./thermalCam** pour prendre une photo. L'image prise par la caméra classique est écrite dans le fichier **test.bmp** et l'image éditée avec les informations de température est écrite dans le fichier **testIR.bmp**


## Boîtier
Le modèle du boîtier a été récupéré sur GrabCAD ([disponible ici](https://grabcad.com/library/laser-cut-wood-case-for-raspberry-pi-3-1)) puis modifié pour être adapté au bois disponible au FabLab

## Auteurs
- [Yann Ducruy](https://github.com/yannou38)
- [Rémi Segretain](https://github.com/rsegretain)
