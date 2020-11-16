# Sensors #

This entire folder is included into the "sensor"-integration. Each file is briefly described here. But at first here is a short list, which sensor-platform I'm using:

- **template** - used for attribute extraction and calculations
- **moon** - used for get information about the current moon phase
- **darksky** - used to get detailed weather information
- **systemmonitor** - used to get information about the host machine
- **time** - used to get the current time as a sensor
- **dwd_weather_warnings** - used to get weather warnings

## bed_weight.yaml ##

As decribed *here* im using HX711-Sensors to monitor the current weight laying in bed. As our bed has 8 feet I need two sensors, which values need to be added to a total weight.

This and the case distinction is handled in this file. A good explination and tutorial on this can be read [here](https://selfhostedhome.com/diy-bed-presence-detection-home-assistant/).

## days_until.yaml ##

In this file I'm creating template sensors which display a countdown to a specific date, at the moment there is only christmas. This information is displayed as random fact on the led_sign.

## garbage_collection.yaml ##

I've got an calender for garbage_collection events only. The problem with these sensors is, that the next event is always present no matter how far its away. To work around this I created a sensor, that show 'true' if one of those garbage_events is is on the next day.

## home_count.yaml ##

This sensor show the percentage of all residents that are home. It is mainly to do not trigger unnecessary "monitor" scans. The source of this sensor can be found [here](https://github.com/DubhAd/Home-AssistantConfig/blob/live/sensors/home_count.yaml).

## opentherm.yaml ##

This sensors extracts the current "set"-temperature from my HVAC. It does not work at the moment...

## vacuum.yaml ##

This sensor extracts the battery status from my vacuum robot.