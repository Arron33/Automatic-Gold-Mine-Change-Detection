# Automatic-Gold-Mine-Change-Detection

https://code.earthengine.google.com/a1d57ef6aa98be16d91b4039508ce652

Currently furthering my masters project by developing my code into an interactive web application for automatic gold mine change detection.

The current program automaticaly generates a training dataset using the ESA WorldCover Map and a 2020 median composite. Relivant incidies and slope and elevation infomation is added. Principal componant analysis of the band DN values is computed and added. These Sentinel 2 median composites are then masked using a cloud classifier (SVM) trained of data provided by Elsy Ibrahim et al, 2021. This automaticaly generated training data is then used to train a Random Forest classifier. Once image classification of several dates is completed, pixel change is calculated and outputted at a binary change image. The code allows for analysis of pixel change of any ESA WorldCover class, for any Sentinel 2 image, within any defined polygon globaly.

The code is accesible through the link above (given the user has a Google Earth Engine account) or via the text file in this repo.

Bellow is a figure from my masters project to demonstrate some of my programs results.

![Figure](https://github.com/Arron33/Automatic-Gold-Mine-Change-Detection/blob/3a3163310674d924002e37b57dcd305192605b12/Figure.jpg)
