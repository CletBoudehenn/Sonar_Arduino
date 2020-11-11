<img src="https://i.pinimg.com/originals/62/13/46/62134608fbd069d4386232dba878d340.jpg"/>

# Real-time GPS jamming and spoofing detection with machine learning

These programs make it possible to determine in real time, with machine learning methods, if a GPS receiver is subject to spoofing or jamming.

## Compatibility

`pynmea2` is compatible with Python 2.7 and Python 3.7+

![Python version](https://img.shields.io/pypi/pyversions/pynmea2.svg?style=flat)

## Installation & Requierment
The use of these programs requires the installation of the following python libraries : 

* numpy
* pynmea2
* math
* json
* sklearn

the "pynmea2" package available via this link : https://github.com/Knio/pynmea2

You can install all necessary libraries by executing this command : 

```sh
pip3 install requierement.txt
```

## Use  : 

These programs can run on simulated GPS systems within a simulation platform. 
In our case, we used the navigation simulator: "BridgeCommand", the electronic map display "OpenCPN" with an embedded plugin called "tactics".

BridgeCommand is available at this address : https://www.bridgecommand.co.uk/Download

OpenCPN is available at this address : https://opencpn.org/OpenCPN/info/downloads.html

### Description : 

1. [statistical_method] this method implements and evaluates the different functions related to the statistical resolution of the problem.

* If you want to use the satistical method, you can use this command : 

```sh
python3 main.py
```

2. [SVM_LOF_method] this method implements and evaluates (via svm or lof based on sklearn libaray) to detect jamming or spoofing

* If you want to use the svm anomaly detection method with scoring, you can use this command : 

```sh
python3 score_SVM.py
```

3. [real_time_detection] this script contains the "ready to use" realease of these two types of scripts

* To execute the script based on svm for real-time analysis, you can use the command : 

```sh
python3 real_time_detection.py
```

4. [man_in_the_middle] This programm generates a Man_In_The_Middle between BirdgeCommand and OpenCPN. You just have to set the right ports and ip address for the sockets. Then the script will modify the latitude and longitude data of the ship in real time before sending them to the electronic chart display simulation system.

* If you want to use the man_in_the_middle script (With BridgeCommand and OpenCPN), you can use this command : 

```sh
python3 man_in_the_middle.py
```

5. [predictions] These two programs can predict and determine whether a test data set is subject to decoy or interference using different features. For example by analyzing variations in phi and g or variations in distance and heading.

* If you want to make some predictions with your own dataset by using these scripts, you can use : 

```sh
python3 prediction.py
```

## Disclaimer

### :exclamation: These programs have been produced as part of an end-of-study project, they are not intended to be used in any other context than the pedagogical one. 
### :exclamation: The authors of these programs are not responsible for the misuse of these scripts and their functionalities. 
### :exclamation: They have been tested in a supervised environment by specific professionals.
