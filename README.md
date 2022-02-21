# QuasarMorphCNN
CNN models for Quasar morphology classifications

Article, cite: https://arxiv.org/abs/2201.09901


## Introduction
CNN models are built for classifying quasar sources with Integrated flux density at 1.4 GHz > 2mJy. Image cutouts (4'x4') are obtained from VLA FIRST image cutout server (https://third.ucllnl.org/cgi-bin/firstcutout), with source SDSS coordinates at the center of the image. 

Sources are classified as core, double, triple, and jets. Core-type sources are subclassified into resolved and unresolved core sources. The models are used to classify radio morphology of 16491 sources.

##### Class and Sub-class Notations:<br/>
core: core-type sources<br/>
double: double-type sources<br/>
trip: triple-type sources (double-lobed)<br/>
jet: jet-type sources<br/>

r: resolved core<br/>
u: unresolved core<br/>
l: lobe-dominated <br/>
c: core-dominated<br/>

## A) CNN models<br/>
1. Three CNN model files have been added to the folder named 'CNN'.<br/>
2. You can load the model files using keras and tensorflow packages.<br/>
3. The input file details along with the labels can be found in the .pickle files. Files beginning with 'X' consists of the image information, while the ones with 'y' contain the corresponding morphology label.<br/>

### A1) MainClass<br/>
CNN model to classify sources into core, lobe, triple and jets. <br/>
### A2) Double<br/>
CNN model to subclassify Double-type sources into core-dominated and lobe-dominated sources.<br/>
### A3) Triple<br/>
CNN model to subclassify Triple-type sources into core-dominated and lobe-dominated sources.<br/>


## B) Broad Absorption Line (BAL) Quasars <br/>
BAL quasars are studied as a function of radio-loudness and core-lobe flux density ratio parameters. These parameters have been compiled for 16491 sources in the "balcatalog.csv" file.<br/>



Flags:<br/>

<b>CLASS</b>: Defines broad classification of radio morphology<br/>
<b>SUBCLASS</b>: Defines sub-classification of radio morphology<br/>
<b>logR1</b>: Log(R<sub>I</sub>) parameter (radio-to-optical ratio)<br/>
<b>logR_ratio</b>: Log(R) parameter (core-to-lobe flux density ratio)<br/>


## Classified Images

### 1) Main Classification Examples
![main2](https://user-images.githubusercontent.com/78647966/139008403-abd8c16c-3018-49e9-914b-9a90705780a1.jpg)

### 2) Sub-Classification Examples
![sub2](https://user-images.githubusercontent.com/78647966/139010395-61977376-973a-41d9-9ee3-21cf1ba126e6.jpg)

