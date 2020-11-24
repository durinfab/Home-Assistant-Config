# Device Tracker  #

This entire folder is included into the ["device_tracker"-integration](https://www.home-assistant.io/integrations/device_tracker/). Each file is briefly described here. But at first here is a short list, which sensor-platform I'm using:

- **[mqtt](https://www.home-assistant.io/integrations/device_tracker.mqtt/)** - Used to translate mqtt messages to device_tracker devices 🏠
- **[nmap_tracker](https://www.home-assistant.io/integrations/nmap_tracker/)** - Used to scan for the presence WiFi devices 📲

## monitor.yaml ##

All devices, which are observed are represented by a MQTT topic (configured by the "monitor" software). These are referred here. The idea and parts of the realisation are from [here](https://github.com/DubhAd/Home-AssistantConfig/tree/live/device_tracker).

## mqtt_person.yaml ##

This file tracks the location state of each resident. These states are the result of a reliable function from [here](/config/automations/presence/fabi_presence.yaml). These location states reflects the assumption if a resident is home. The idea of the implementation of this file is [here](https://github.com/DubhAd/Home-AssistantConfig/blob/live/device_tracker/mqtt_person.yaml).  

## nmap_tracker.yaml ##

This file tracks the necessary WiFi-Devices, such as mobile phone and smart watches, which are needed by the presence detection. Please mention that WiFi is not as reliable as Bluetooth, because most devices disconnect from WiFi when they don't need it. These can lead to a wrong assumption corresponding their presence. The idea of the implementation of this file is [here](https://github.com/DubhAd/Home-AssistantConfig/blob/live/device_tracker/nmap_tracker.yaml).  