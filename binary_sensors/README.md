# Binary Sensors  #

This entire folder is included into the ["binary_sensor"-integration](https://www.home-assistant.io/integrations/binary_sensor/). Each file is briefly described here. But at first here is a short list, which sensor-platform I'm using:

- **[mqtt](https://www.home-assistant.io/integrations/binary_sensor.mqtt/)** - Used to translate mqtt messages to binary_sensors 🖌
- **[iss](https://www.home-assistant.io/integrations/iss/)** - get current information about the ISS 🛰

## monitor_devices/ ##

Tracking of the Online status of my "monitor"-devices. If they are offline for a long time, [they get resetted](/config/automations/presence/bt_first_floor.yaml).

## iss.yaml ##

A sample information source for the random information. We can track if the iss is above our local location and print the count of currently present people there 👩🏼‍🚀

Currently not used.

