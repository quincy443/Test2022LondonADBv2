# Project Umbrella 2022
## OBJECTIVE

### Question:

In Hong Kong existing Chinese tenements (Tong Lau) built before 1930 are rare, and thus historical and precious; those multi-storey tenements made of reinforced concrete are taller and relatively common. They still contribute to our everyday urban sensual experiences. The technical objective is to measure the height of the various roofs, or verandah, of these Chinese tenements, meanwhile transforming live data into sonic experience.

### Answer:

The initial solution is that any low budget LIDAR device controlled by Arduino could get the job done. 
Final solution here, however, is less demanding on the hardware knowledges. Terabee distance sensor 
prefabricated with Android API indeed also has the advantage of using less disturbing infra-red ray.

## The APP
### [DOWNLOAD](https://play.google.com/store/games?hl=en&gl=US)
 
<img src="https://i.ibb.co/NsGNQdx/app-screenshot.jpg" width="250" border="0">

_APP screenshot_

||  |
|---|--------------- |
|1. | sensor on/off |
|2. | detected distance|
|3. | bubble level|
|4. | bubble level on/off |
|5. | wavelength frequency gain |
|6. | wave form |
|7. | generated wavelength frequency range |
|8. | detected distance range |
|9. | maximum distance |
|10. | live frequency wavelength |
|11. | sound recorder |
|12. | message log |


### A. Distance Sensor _(1)(2)_ 

Terabee Distance sensor is connected to the smartphone via USB cable. The tested sensor has a maximum range of 60 meter. Personal observation concluded that the height of the extended roof of Chinese tenements in Hong Kong is below 12 meters.

### B. Bubble Level _(3)(4)_ 

As the user needs to be in a constant pace walking to operate the app, bubble level, which is based on internal built-in accelerometer of 
common smartphones, is to guide the user to keep phone lay as flat as possible in order to acquire relatively accurate data. 

### C. Sonic Input / Output Parameters _(7)(8)(9),(6)_

Live distance data feed whose range of diatance (in meters) is estimated in advance at sites. 
The range of distance will be correpsonded straightforwardly to desirable range of sound determined solely by its wavelength. 
The waveform has the options of sine, triangular, sawtooth and pulse. User could change the option by touching on the waveform image _(6)_.

### D. Recording _(11)(7)_

Two files are created when the reocording feature is invoked, which 
are accessible at _/android/data/com.distance2noise/files/audio/_ :

### 1. .wav audio file _(7)(8)(5)_ 
>This is a simple audio file in uncompressed .wav format which was recorded by the APP
>  
>Filename example:
>_aud211130_081256d0106f00402500g3.wav_
> 
>|aud| 211130_081256|d|0106|f|f00402500|g|3|.wav |
>|---|--------------|-|----|-|---------|-|-|---- |
>|   | 2021 Nov 30 8:12:56|distance|1-6m|frequency|40 - 2580Hz|amplitude gain|x3| |
>
### 2. .csv file  
>The csv file contains distance data from live feed via distance sensor.
>   
>Filename example:
>_dis211130_081256.csv_
> 
>|dis| 211130_081256|.csv |
>|---|--------------|---- |
>|   | 2021 Nov 30 8:12:56| |
>   
>Regardless of data bandwidth, distance in meter will be constantly
>recorded 600 times per minute.

>Data format of the csv is simply as follows:
>   
>|line| value |
>|---|---------- |
>| 1  | Creation Timestamp (hhmm_hhssmm) |
>| 2  |  distance 1 |   
>| 3  |  distance 2 |   
>| 4  |  ... |   
>   
>Heights of the roof of different Chinese tenements along the pedestian pathways could thus be visualized 
>as distance data could be remapped, easily by Google Sheets, as chart like the following:
>
>#### Example Visualized Distance Chart (based on .csv file)
><img src="https://i.ibb.co/R4DTWF4/sketch-1662554043749.jpg" height="250">
>
>


## Tested Platform and Hardware

Operating System: Android 8.0.0 

Distance Sensor : Terabee TeraRange Evo 60m 

## References

>[AAudio Engine](https://developer.android.com/ndk/guides/audio/aaudio/aaudio)

>[.WAV Soundfile Format ](http://soundfile.sapp.org/doc/WaveFormat/)






