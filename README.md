# Anomaly detection using statistical change detection 

## Table of content
* Motivation
* Dataset
* Tools used for the project
## Motivation
This project seeks to evaluate different algorithmic solutions to detect online flux jumps in The Large Hadron Collider (LHC), designed and put into operation by CERN (Organisation Européenne pour la Recherche Nucléaire) in 2008, is a large ring of 27 km, built at 100 meters below the earth’s surface, where 2 beams of protons can be accelerated at nearly the speed of light and collided in massive detectors where particles created by the collision can be identified. LHC was built to assist scientists in their quest to answer questions about the universe's creation by, for instance, discovering new particles such as the Higgs boson.

The algorithms tested are statistical change detection algorithms using sliding windows.
In the folder, Data is the subfolder Jumps which contains 6 CSV files, recordings of the magnetic flux measured on a supra-conducting magnet. 
The Signals folder contains data on the magnetic flux. each dataset is sampled at a rate of 5ms.  This signal has a zero mean. It measures the difference between the flux and its reference.
s(number).flux is a boolean signal of the same length as s(number).signal. When s(number).flux is equal to 1, a flux jump is present. s(number).flux thus localizes periods of time when a flux jump occurred.

## Tools used for the project

This repo is in python 
