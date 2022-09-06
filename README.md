# Test2022LondonADBv2
description for 2022 London ADB Haha

APP Objective

illustration
 
APP screenshot

Sensor On/Off
Detected Distance
Levelmeter
meter Display/Hidden
wavelength frequency gain
wave form
generated wavelength frequency Range
Detected Distance Range
live frequency wavelength
Sound Recorder
Message Log

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

Source References
AAudio Engine
.wav file writer 


