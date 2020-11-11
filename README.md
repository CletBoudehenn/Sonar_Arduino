<img src="https://i.pinimg.com/originals/62/13/46/62134608fbd069d4386232dba878d340.jpg"/>

# Real-time GPS jamming and spoofing detection with machine learning

These programs make it possible to determine in real time, with machine learning methods, if a GPS receiver is subject to spoofing or jamming.

Requierment :

## Compatibility

`pynmea2` is compatible with Python 2.7 and Python 3.4+

![Python version](https://img.shields.io/pypi/pyversions/pynmea2.svg?style=flat)

## Installation 
The use of these programs requires the installation of the following python libraries
notamment l'utilisation de la lib "pynmea2" disponible via ce lien : https://github.com/Knio/pynmea2

Vous pouvez installer toutes les lib nécéssaire en executant directement cette commande : 

```sh
pip3 install requierement.txt
```

## Use  : 

These programs can run on simulated GPS systems within a simulation platform. 
In our case, we used the navigation simulator: "BridgeCommand", the electronic map display "OpenCPN" with an embedded plugin called "tactics".

BridgeCommand is available at this address : https://www.bridgecommand.co.uk/Download

OpenCPN is available at this address : https://opencpn.org/OpenCPN/info/downloads.html

### Description : 

1. [Statistical Method] which implements and evaluates the different functions related to the statistical resolution of the problem.
2. [SVM_LOF method] which implements and evaluates several atrificial intelligence methods (via python's scikit-learn module) to determine the presence or absence of decoys.
3. [Script_final method] which contains the "ready to use" version of these two types of scripts

To execute le script, you can use the command : 

```sh
python3 detection_temps_reel.python3
```
