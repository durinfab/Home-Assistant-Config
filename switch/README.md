# Switches #

This entire folder is included into the "switch"-integration. Each file is briefly described here. But at first here is a short list, which switch-platforms I'm using:

- **template** - used (atm) only to integrate unsupported hardware to HomeKit.
- **circadian_lighting** - every light group gets its own switch. Used to dis- /enable the color adjustment.
- **wake_on_lan** - used to wake up corresponding devices from sleep

At the moment, I'm not using that much switches...

## homekit_switches.yaml ##

Some integrations, as my vaccuum robot, are not supported by HomeKit. But because of the easy access with Siri I want them still there. Thats why im adding a custom switch that starts the vaccuum robot and calls him back.

## circadian_lighting.yaml ##

All circadian_lighting-switches used in my Smart Home. For a more detailed explanation look [here](https://github.com/claytonjn/hass-circadian_lighting).

## **wake_on_lan.yaml** ##

As the name says, here are all my wake_on_lan switches. At the moment I'm only treat my Living Room PC at the moment.