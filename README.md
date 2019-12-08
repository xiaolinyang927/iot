# iot
Weather Station with Raspberry Pi
## Introduction:
      Use BME280 sensor to measure the tmeperature, humidity and pressure. Then send the data to the Google Sheet.
## hardware:
      A Raspberry Pi 3B+
      A BME280 pressure, temperature, and humidity sensor
## Software:
### The Oracle Raspberry Pi Weather Station software. Don’t need to install it, just use some of the Python programs.
      'git clone https://github.com/RaspberryPiFoundation/weather-station'
### The BME280 Python library
      'sudo pip3 install RPi.bme280'
## BME280:
      The BME280 sensor is a digital sensor that can measure temperature, humidity, and atmospheric pressure. It is
      available in a number of breakout boards from popular manufacturers such as Adafruit. One thing to check is 
      that the I2C address is correct: for the Adafruit models it is 0x77 (as shown in the code below), but other 
      versions can have different addresses (0x76 is a common alternative).
###   Pi GPIO	BME280
      17 (3V3)	Vin  
      6 (Gnd)	Gnd  
      3 (SDA)	SDA (SDI)  
      5 (SCL)	SCL (SCK)  
      Some other breakout boards may have other pins (such as SDO or CSB), but those are not generally needed.
