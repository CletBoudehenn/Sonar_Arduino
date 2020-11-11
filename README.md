<img src="https%3A%2F%2Fwww.youtube.com%2Fwatch%3Fv%3D4iNThvr8nvM&psig=AOvVaw31AbKxYRXkPld9ipgjJhZ_&ust=1605198768868000&source=images&cd=vfe&ved=2ahUKEwik28jE9frsAhVuAWMBHUHFBWwQjRx6BAgAEAc"/>

# Détection en temps-réel de brouillage opu leurrage GPS avec des méthodes d'apprentissage automaique 

Ces programmes permettent de déterminer en temps réel, grâce a des méthodes d'apprentissage automatique, si un récepteur GPS est soumis à du leurrage ou du brouillage.

Requierment :

## Installation 
L'utilisation des ces programmes nécessite l'installation des quelques libraries python
notamment l'ulisation de la lib "pynmea2" disponible via ce lien : https://github.com/Knio/pynmea2

Vous pouvez installer toutes les lib nécéssaire en executant directement cette commande : 

```sh
pip3 install requierement.txt
```

## Utilisation : 

Ces programmes peuvent fonctionner sur des systèmes GPS simulé au sein d'une plateforme de simualtion. 
Dans notre cas, nous avons utilisé le simulateur de navigation : "BridgeCommand", l'afficheur de carte electronique "OpenCPN" et la version 3.8 de python.

BridgeCommand est disponible à cette adresse : https://www.bridgecommand.co.uk/Download

OpenCPN est disponible à cette adresse : https://opencpn.org/OpenCPN/info/downloads.html

### Dans ce dépôt, il y a 3 techniques distinctes : 

1. [Méthode Statistique] qui implémente et évalue les différentes fonctions relatives à la résolution statistique du problème
2. [Méthode SVM_LOF] qui implémente et évalue plusieurs méthodes d'intelligence atrificielle ( via le module scikit-learn de python ) pour déterminer la présence ou non de leurrage.
3. [Méthode script_final] qui contient la version "prête à l'emploi" de ces deux types de scripts

Pour écxécuter les script, vous pouvez utiliser la commande : 

```sh
python3 detection_temps_reel.python3
```
