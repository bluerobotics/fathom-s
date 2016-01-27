#Fathom-S

The Fathom Tether Boards are part of Blue Robotics' *Fathom Tether*. These boards provide interfaces and functionality for the communication methods used with the tether. With the Fathom tether, it is quick and easy to get up and running and interface with your ROV or other application.

The schematic and board layout are designed in EagleCAD.

#Fathom-S (Serial) Hardware

##Description

The Fathom-S Hardware is designed for applications using a simple microcontroller for ROV control. It is meant to be an all-inclusive tether interface. The power switching capability allows small ROVs to be completely powered through the switched battery power connection with 20A continuous and 40A burst current ratings. Larger systems with higher current or voltage requirements must use an external power switching circuit or rely on plug/unplug power systems.

The Fathom-S Hardware is designed to be used with tether cables that have four twisted pairs, preferrably similar to Cat5 cable. The design is based on the tether cables available from Blue Robotics, but will also work with standard Cat5 network cable.

##Features 

* Low Latency Analog Video through NTSC or PAL (1000+ ft, 300+ m)
* Full-duplex RS-422 serial connection with TTL and USB connections (up to 250 Kbps, 4000 ft, 1200 m)
* Power switch that uses a 3-50V input signal to connect batteries and provide up to 20A continuous, 40A burst current
* Onboard 5V and 12V (camera) regulated supplies
* Jumpers to enable/disable configuration options
	* Power-on through tether / power always on when batteries connected
	* Power board from battery / power board from alternate input
	* Power cycle on USB RTS signal for Arduino programming
* 0.1" I/O header for ribbon cable to ROV controller
* Current and voltage sense outputs

##Configuration

###Fathom-S Onboard

[Image with arrows]

###Fathom-S Topside

[Image with arrows]

##Electrical Ratings

| Value                              | Minimum | Nominal | Maximum | Unit    |
|-----------------------------------:|:-------:|:-------:|:-------:|:--------|
| Battery Input Voltage              | 7       | 12      | 26      | V       |
| Power-on Signal Voltage            | 3       | 5       | 50      | V       |
| Switched Battery Output Current    |         | 20      | 40      | A       |
| 5V Regulator Current @ 12V input   |         |         | 250     | mA      |
| 5V Regulator Current @ 26V input   |         |         | 100     | mA      |
| 12V Regulator Current @ 12V input  |         |         | 1000    | mA      |
| 12V Regulator Current @ 26V input  |         |         | 150     | mA      |

##Example Setups

Examples TBD

##Physical Specifications

Dimensions, screw holes, wire gauges, etc.

##APM/PixHawk Adapter Board

The APM/PixHawk Adapter Board allows the Fathom-S board to be interfaced directly to an APM2.6 or PixHawk and many other similar autopilot boards. The following connectors are available:

* Telemetry serial port to the tether RS422 serial port (via DF13 connector)
* Power to the power plug including voltage and current monitoring (via DF13 connector)


##License

The Fathom Serial Hardware Design is released under the MIT License.

##Revision History

0.0 - Under development. Not fully functional.

0.1 - Second prototype. Not fully functional.

0.2 - Third prototype. First beta release - works great.