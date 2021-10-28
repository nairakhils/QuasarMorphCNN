# QuasarMorphCNN
CNN models for Quasar morphology classifications


## Introduction
CNN models are built for classifying quasar sources with Integrated flux density at 1.4 GHz > 2mJy. Image cutouts (4'x4') are obtained from VLA FIRST image cutout server (https://third.ucllnl.org/cgi-bin/firstcutout), with source SDSS coordinates at the center of the image. 

Sources are classified as core, double, triple, and jets. Core-type sources are subclassified into resolved and unresolved core sources. The models are used to classify radio morphology of 16491 sources.

##### Class and Sub-class Notations:
core: core-type sources
double: double-type sources
trip: triple-type sources (double-lobed)
jet: jet-type sources

r: resolved core
u: unresolved core
l: lobe-dominated 
c: core-dominated

## A) CNN models
1. Three CNN model files have been added to the folder named 'CNN'.
2. You can load the model files using keras and tensorflow packages.
3. The input file details along with the labels can be found in the .pickle files. Files beginning with 'X' consists of the image information, while the ones with 'y' contain the corresponding morphology label.

### A1) MainClass
CNN model to classify sources into core, lobe, triple and jets. 
### A2) Double
CNN model to subclassify Double-type sources into core-dominated and lobe-dominated sources.
### A3) Triple
CNN model to subclassify Triple-type sources into core-dominated and lobe-dominated sources.


## B) Broad Absorption Line (BAL) Quasars 
BAL quasars are studied as a function of radio-loudness and core-lobe flux density ratio parameters. These parameters have been compiled for 16491 sources in the "balqso.csv" file.
Flags:
CLASS: Defines broad classification of radio morphology
SUBCLASS: Defines sub-classification of radio morphology
logR1: Log(RI) parameter (radio-to-optical ratio)
logR_ratio: Log(R) parameter (core-to-lobe flux density ratio)


## Classified Images

### 1) Main Classification Examples
![main2](https://user-images.githubusercontent.com/78647966/139008403-abd8c16c-3018-49e9-914b-9a90705780a1.jpg)

### 2) Sub-Classification Examples
![sub2](https://user-images.githubusercontent.com/78647966/139010395-61977376-973a-41d9-9ee3-21cf1ba126e6.jpg)

