# Project Umbrella 2022
## OBJECTIVE

### Question:

As one walks along the streets in Hong Kong, how to measure the height of the various "roofs" of the buildings, and simultiously
transform it into sonic experience?

### Answer:

The initial solution is that any low budget LIDAR device controlled by Arudino should get the job done. 
Our solution here, however, is less demanding on the hardware knowledges; Using Terabee distance sensor 
prefabricated with Android API indeed has the advantage of using non-disturbive infra-red ray.

<img src="https://i.ibb.co/NsGNQdx/app-screenshot.jpg" width="250">
##### APP screenshot

1. Sensor On/Off
2. Detected Distance
3. Levelmeter
4. meter Display/Hidden
5. wavelength frequency gain
6. wave form
7. generated wavelength frequency Range
8. Detected Distance Range
9. live frequency wavelength
10. Sound Recorder
11. Message Log

input

bubble level to keep phone lay flat



output control



## Output Files

Two files are created when the reocording feature is invoked, which 
are accessible at _/android/data/com.distance2noise/files/audio/_ :

### 1. .wav audio file
 
   This is a simple audio file in uncompressed .wav format which was recorded by the APP
  
   Filename example:
   _aud211130_081256d0106f00402500g3.wav_
 
|aud| 211130_081256|d|0106|f|f00402500|g|3|.wav |
|---|--------------|-|----|-|---------|-|-|---- |
|   | 2021 Nov 30 8:12:56|distance|1-6m|frequency|40 - 2580Hz|amplitude gain|x3| |

### 2. .csv file  
   The csv file contains distance data from live feed via distance sensor.
   
   Filename example:
   _aud211130_081256.csv_
 
|dis| 211130_081256|.csv |
|---|--------------|---- |
|   | 2021 Nov 30 8:12:56| |
   
   
   Regardless of data bandwidth, distance in meter will be constantly recorded 600 times per minute.
   
   Data format of the csv is simply as follows:
   
      creation timestamp (hhmm_hhssmm)
      distance 1 
      distance 2
      ...
    
    Various heights of the "ceiling" along the pedestian street could thus be visualized 
    as distance data could be remapped, easily by Google Sheets, as chart like the following:

<img src="https://i.ibb.co/R4DTWF4/sketch-1662554043749.jpg" height="250">
#### _visualized distance chart based on .csv file_

ENGLISH 
see Terabee implement


## Tested Platform

Operating System: Android x.0 (tested)

Distance Sensor : Terabee TeraRange Evo X0 

## Source References

This site was built using [GitHub Pages](https://pages.github.com/).

rundown [tutorial](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)

AAudio Engine

.wav file writer 




