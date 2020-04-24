# OpenRobot

OpenRobot is an Open Hardware PCB based on Arduino Nano, especially designed for teaching technology

Once assembled, you can use make multiple projects and robots without welding, just adding or removing components in the dupont headers.


![alt text](https://github.com/luisllamasbinaburo/OpenRobot/blob/master/OpenRobot/Images/OpenRobot-schematic.jpg "Assembly")


OpenRobot is compatible with a huge number of modules thanks to the multiple outputs. 
Also, is compatible with several DC Converters, and differents IMUs (MPU6050, MPU9050/9250 and L3GD20)

## What can I make with OpenRobot?
Almost any Arduino project you can ever imagine! 

![alt text](https://github.com/luisllamasbinaburo/OpenRobot/blob/master/OpenRobot/Images/OpenRobot-assembly.jpg "Assembly")



Some of them,
- DC Motors Robot, like obstacle avoider (ultrasonic or Sharp), line follower, self-balancing bot...
- Servo Motor Robot, like 2-DOF Tower, 6-DOF Arms...
- Mosfet output for high current proyects (LED, electromagnets, water pumps)
- Bluetooth projects (HC-05/HC-06), like Android or PC communication, beacons...
- WiFi projects (ESP01), like controlling from Web, MQTT datalogger...
- Temperature, pressure, humidity weather station with BME280
- Any other project, thanks to the multiple available outputs!


## Connectors
A lot of connectos availble, so you can customicce OpenRobot to you project requirement
![alt text](https://github.com/luisllamasbinaburo/OpenRobot/blob/master/OpenRobot/Images/OpenRobot-connectors.png "OpenRobot Connectors")

- 2x DC Motor
- 2x Encoder
- Aux Output 3V3, 5V, Vreg
- 2x I2C 5V + 1x I2C 3V3
- 3x Ultrasonic Sensor
- 3x Analog Input (with optional smd resistor)
- 6x Servo
- 5x IR Sensor
- 3x Mosfet
 
 But, I you wany, can also use any of this output as a GPIO.

## Pinout
Of course, not all the components and outputs are available at the same time, due to Arduino Nano pins numbers.

You have to choose which of this components your project requires. But posibilities are almost ilimited!

This is the pinout of OpenRobot

![alt text](https://github.com/luisllamasbinaburo/OpenRobot/blob/master/OpenRobot/Images/OpenRobot-pinout.png "Pinout")

## Components
OpenRobot allows you to mount several modules to your projects,
- Motor Driver TB6612FNG
- IMU (compatible with several IMUs)
- Temperature/Pressure/Humidity (BMP280/BME280)
- Level shifter (required to use Bluetooth or ESP01)
- Blueooth ESP01
- Bluetooth HC-04/05/06

![alt text](https://github.com/luisllamasbinaburo/OpenRobot/blob/master/OpenRobot/Images/OpenRobot-components.png "Components")

But you can add a lot of modules thanks to the 3V3 and 5V I2C and UART.



## Powering
Powering is one of the most important point in any project. OpenRobot allow a simple but flexible power management in the proyect
- Power Switch 
- Up to 3 DC Converters (5V, 3V3, +1 Vreg)
- Power selector to select wich components (DC Motors, servo, Mosfet) are powering with each DC converter
- Posible to by-pass DC Converters and powering through Nano regulators (just in low-power and simple projects)
- Battery sense (optional)

### DC Converters
OpenRobot is compatible with two different DC Converters modules.

![alt text](https://github.com/luisllamasbinaburo/OpenRobot/blob/master/OpenRobot/Images/OpenRobot-dc-converters.jpg "OpenRobot DC Converters")


Just assembly in the right position for you DC Converter model.
![alt text](https://github.com/luisllamasbinaburo/OpenRobot/blob/master/OpenRobot/Images/OpenRobot-Power.png "OpenRobot Power")


### Power selection
Powering selection to device are make using dupong jumper connections.
Outputs to:
- Servo
- DC Motors
- Mosfet

Can be connected to:
- Vregulated
- 5V
- Vbatery

![alt text](https://github.com/luisllamasbinaburo/OpenRobot/blob/master/OpenRobot/Images/OpenRobot-Power-selector.png "OpenRobot Powering")

Aditionally, you can completely by-pass DC converters, and use Arduino regulators for 3V3 and/or 5V PCB rails, thus removing the need of installing DC Converters at all.

Only recommended in case of small / low power projects

## IMU
IMU is an important part of most Arduino projects. OpenRobot is compatible with a big number of IMUs, including the most populars. 

![alt text](https://github.com/luisllamasbinaburo/OpenRobot/blob/master/OpenRobot/Images/OpenRobot-IMUs.jpg "OpenRobot IMUs")

Just put your IMU in the right position. In some IMU modules you make need to use the Vcc optional pin to adapt powering to your IMU pinout.

![alt text](https://github.com/luisllamasbinaburo/OpenRobot/blob/master/OpenRobot/Images/OpenRobot-IMU.jpg "OpenRobot IMU")


