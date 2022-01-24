# OakDLiteContest_GeoFence
repository for the OpenCV Spacial AI Contest using the OakD Lite. We are developing a Livestock and Pet Geofence that is an autonomous system that monitors animals within a zone.

## Team: SoFlo Primary Key

## Problem Statement
Monitoring livestock and pets within a zone can be a struggle. Traditional fences can be broken while leaving the owner unaware that their animals are loose. Loose animals can lead to property damage, loss of the animal, panic, and heartbreak. We propose an autonomous system that can monitor animals and send notifications when animals have crossed a boundary line of a predetermined zone.

This system consists of an autonomous module and a base station. The autonomous module is comprised of the Oak-D Lite camera, a pan and tilt base, a Raspberry Pi with GPS, IMU, and LoRa. The autonomous module would ideally be suspended by a zipline trolley. The zipline trolley allows the system to monitor a much larger zone. The system can also be affixed atop a good vantage point for smaller zones.

The base station is used to set the boundary of the zone and to relay LoRa notifications from the autonomous module to a wireless local area network. Notifications can be received by the user’s mobile device. The user may setup the zone by entering GPS coordinates or by printing out and placing ArUCo markers at the vertices of the zone. The ArUCo markers would only be needed during the setup process and afterwards they can be removed.

The out of zone detection pipeline detects the presence of an animal, classifies its species, tracks it, and compares its present location to the zone’s mask. The animal classification stage is optional and is utilized by users who want to detect unwanted animals.


This is a higher-level library to allow Adafruit's [CLUE](https://www.adafruit.com/product/4500) and ElecFreak's micro:bit Smart [Cutebot](https://www.elecfreaks.com/micro-bit-smart-cutebot.html) to communicate while maintaining all the functionality of the CLUE, except for touch features. In version 2, the code has been updated for efficency purposes and educational focus has shifted towards examples and wiki.

## Dependencies
This library depends on:
* [Adafruit CircuitPython](https://github.com/adafruit/circuitpython) v.5.3.1
* [Adafruit_hcsr04](https://github.com/adafruit/Adafruit_CircuitPython_HCSR04)

The IR remote example also depends on:
* [Adafruit_irremote](https://github.com/adafruit/Adafruit_CircuitPython_IRRemote)

The Adafruit BlueFruit Connect App's Controller example also depends on:
* [Adafruit_ble](https://github.com/adafruit/Adafruit_CircuitPython_BLE)
* [Adafruit_bluefruit_connect](https://github.com/adafruit/Adafruit_CircuitPython_BluefruitConnect)

## License
The code of the repository is made available under the terms of the MIT license. See license.md for more information.
