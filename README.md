# Test2022LondonADBv2
## description for 2022 London ADB Haha

APP Objective

illustration
 
 ![screenshot](https://i.ibb.co/9V31cZp/app-screenshot.jpg)
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
output
.wav

.csv 
file naming convention


public String composeSuffix(float dist1, float d2, int freq1, int f2, int gain) {
   String suf="";
   suf+="d"+new DecimalFormat("00").format((int)dist1)
           +new DecimalFormat("00").format((int)d2)
           +"f"
           +new DecimalFormat("0000").format(freq1)
           +new DecimalFormat("0000").format(f2)
           +"g"+gain;

   return suf;

ENGLISH 
seeTerabee implement

Android x.0 (tested)

Distance Sensor : Terabee Evo X0 

This site was built using [GitHub Pages](https://pages.github.com/).

rundown [tutorial](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)

AAudio Engine
.wav file writer 


