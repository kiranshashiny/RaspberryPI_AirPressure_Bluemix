# RaspberryPI_AirPressure_Bluemix

The BMP180 Pressure sensor connects to the I2C bus of the Raspberry Pi.

<img width="368" alt="screen shot 2017-02-19 at 1 14 20 pm" src="https://cloud.githubusercontent.com/assets/14288989/23247334/78c544d6-f9bf-11e6-918f-90a8291a6282.png">

To learn more on the I2C bus https://learn.adafruit.com/adafruits-raspberry-pi-lesson-4-gpio-setup/configuring-i2c

These have to be enabled before we connect to the Sensor

First enable the I2C and the SPI bus on the Raspberry pi

I have a RPI 2, and installed with Raspian OS

		cat /etc/os-release

		PRETTY_NAME="Raspbian GNU/Linux 7 (wheezy)"
		NAME="Raspbian GNU/Linux"
		VERSION_ID="7"
		VERSION="7 (wheezy)"
		ID=raspbian
		ID_LIKE=debian
		ANSI_COLOR="1;31"
		HOME_URL="http://www.raspbian.org/"
		SUPPORT_URL="http://www.raspbian.org/RaspbianForums"
		BUG_REPORT_URL="http://www.raspbian.org/RaspbianBugs"


Follow driver installation instructions as listed in this link:

https://learn.sparkfun.com/tutorials/raspberry-pi-spi-and-i2c-tutorial#connecting-to-the-ports


<img width="511" alt="screen shot 2017-02-23 at 11 50 16 am" src="https://cloud.githubusercontent.com/assets/14288989/23247132/4cf59ece-f9be-11e6-983e-56adc3558cd6.png">



Connect the BMP 180 to the Raspberry Pi as follows :

Vcc to 3.3V ( Pin 1 of Raspberry Pi)
SDA to Pin3
SCL to Pin 5
GND to Pin 39 of the Raspberry Pi.


Download the bmp180 python software from this link:

http://www.raspberrypi-spy.co.uk/2015/04/bmp180-i2c-digital-barometric-pressure-sensor/


or simply put:


        wget https://bitbucket.org/MattHawkinsUK/rpispy-misc/raw/master/python/bmp180.py

        sudo python bmp180.py


<img width="489" alt="screen shot 2017-02-23 at 11 53 45 am" src="https://cloud.githubusercontent.com/assets/14288989/23247219/c76e1302-f9be-11e6-81f8-5917abf8911a.png">



