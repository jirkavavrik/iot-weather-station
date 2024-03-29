# iot-weather-station

IoT weather station is an Arduino Nano 33 IoT based weather station that reads data about temperature, humidity and air pressure using sensors SHT30 and BMP180. It then sends them via MQTT periodically to a device running a Node-RED instance taht displays the info on a web dashboard. Node-RED flow is also configured to send the data to Blynk cloud.

## Ignored file should look like this:

### src/arduino_code/arduino_secrets.h
```
#pragma once
#define SECRET_SSID "your ssid"
#define SECRET_PASS "your password"
```
In the Node-RED flow don't forget to rewrite the API_KEY in order to send data to Blynk cloud.

## Photos of the weather station

![Photo 1 of the weather station](doc/photo1.jpg)
![Photo 2 of the weather station](doc/photo2.jpg)

## Screenshots of dashboards
### In Node-RED:
![Screenshot of dashboard in Node-RED](doc/screenshot1.png)
### In Blynk cloud:
![Screenshot of a possible dashboard in Blynk](doc/screenshot2.png)
