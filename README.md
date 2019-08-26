# Ninux Sensor ESP32
General purpose Sensor Client fon Ninux Sensor Network using ESP32 platform

## 


## Requirements

### Hardware Requirements
1. ESP32 Controller
1. LoreWan Module 868MHz
1. Display Oled
1. Reset button 
1. Programmable button

### Software Requirements
1. Configuration Provisioning via Wifi and save parameter in NVRAM 
1. Network connection configurable mode:
   1. Wifi/MQTT only
   1. LoraWan only
   1. Wifi/MQTT - LoraWan failover
   1. LoraWan - Wifi/MQTT failover
1. Display Message helper
1. Deep Sleep Mode
1. Wifi OTA firmware update

## API

### Display Gatekeeper Task
There are two way to write on OLED Diplay:
* Send a command directly on Display Gate Keeper (DGK) Queue
* Create a Selfkiller task that sends a command to DGK Queue 
