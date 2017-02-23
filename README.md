# RaspberryPI_AirPressure_Bluemix


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


Follow instructions as listed in this link:

https://learn.sparkfun.com/tutorials/raspberry-pi-spi-and-i2c-tutorial#connecting-to-the-ports


<img width="511" alt="screen shot 2017-02-23 at 11 50 16 am" src="https://cloud.githubusercontent.com/assets/14288989/23247132/4cf59ece-f9be-11e6-983e-56adc3558cd6.png">



Connect the BMP 180 as follows :

Vcc to 3.3V ( Pin 1 of Raspberry Pi)
SDA to Pin3
SCL to Pin 5
GND to Pin 39 of the Raspberry Pi.



