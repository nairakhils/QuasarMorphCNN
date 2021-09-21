# QuasarMorphCNN
CNN models for Quasar morphology classifications


## Introduction
CNN models are built for classifying quasar sources with Integrated flux density at 1.4 GHz > 2mJy. Image cutouts (4'x4') are obtained from VLA FIRST image cutout server (https://third.ucllnl.org/cgi-bin/firstcutout), with source SDSS coordinates at the center of the image. 

Sources are classified as core, lobe, triple, and jets. Core-type sources are subclassified into resolved and unresolved core sources.

##### Class and Subclass Notations:
core: core-type sources
lobe: lobe-type sources
trip: triple-type sources (double lobed)
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
### A2) Lobe
CNN model to subclassify Lobe-type sources into core-dominated and lobe-dominated sources.
### A3) Triple
CNN model to subclassify Triple-type sources into core-dominated and lobe-dominated sources.



## Classified Images

### 1) Main Classification Examples
![appendixmain1](https://user-images.githubusercontent.com/78647966/134183473-0cac426f-30a8-4559-a3f9-21433088ebea.png)

### 2) Sub-Classification Examples
![appendixsub1](https://user-images.githubusercontent.com/78647966/134183485-e581d657-2fcd-45d7-8197-183c671b52bb.png)
