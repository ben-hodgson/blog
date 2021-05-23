+++
title = "Weather Station"
date = "2021-05-19T15:06:51+01:00"
author = "Ben Hodgson"
authorTwitter = "" #do not include @
cover = ""
tags = ["project", "weather station", "python"]
keywords = ["python", "project", "weather station"]
description = "Weather station project intro"
showFullContent = false
+++

I have been working on a weather station for a little while. Longer than I'd have wanted but with other work and getting the money together to buy the parts its taken a while.
I have had a DHT11 plugged into a breadboard and connected to a Raspberry Pi Zero W for a few months. I have written a program in python to gather the temperature and humidity every 30 minutes. It then writes this data to a .xlsx file.

I have just purchased a BMP280 from Pimoroni to see how well that performs with temperature readings, as I have read about them not being as accurate due to the thermometer being encased in with the other sensors.
I have had some trouble getting it to work on my Raspberry Pi 3b+ and I was beginning to think that it may be faulty. I checked that I2C was running multiple times and I checked that I got a reading of 76 when I ran ```icdetect -a 1``` which I did.
I checked my solder joints and re-soldered one pin. I tried the BMP280 in the Raspberry Pi 0 W and it still didn't work, I was about to give up and thats when I realized that I had cloned and installed the files for a BME280 and not the BMP280.

Thankfully after realizing this mistake I cloned and installed the correct files and it is now working as intended and I can get on with comparing the DHT11 and BMP28. I will run them against each other for the next week to see what differences in readings they
produce and thenI think I will start looking at getting a anemometer designed and 3D printed.

My plan for this weather station is not only for temperature, humidity, pressure and, wind speed readings. But I want to have a rain gauge too and I may also look into the possibility of wind direction
