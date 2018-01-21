# WemosIRLearningRemote
A learning IR remote using the Wemos D1 Mini 

This project is based on the excellent IRremoteESP8266 project by markszabo, here: https://github.com/markszabo/IRremoteESP8266 

It combines two examples in the IRremoteESP8266 project into a single codebase so that both "IR blasting" and "Learning" are implemented in the same MCU unit (Wemos D1 Mini). The two example files are:
https://github.com/markszabo/IRremoteESP8266/blob/master/examples/IRMQTTServer/IRMQTTServer.ino
and
https://github.com/markszabo/IRremoteESP8266/blob/master/examples/IRrecvDumpV2/IRrecvDumpV2.ino

IR codes can be sent to the Wemos via MQTT to activate the IR LED, and shining a remote at the IR Receiver connected to the Wemos generates the corresponding codes and it is returned via MQTT. 
