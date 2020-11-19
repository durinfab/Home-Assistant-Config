# Sensors  #

This entire folder is included into the ["sensor"-integration](https://www.home-assistant.io/integrations/sensor/). Each file is briefly described here. But at first here is a short list, which sensor-platform I'm using:

- **[template](https://www.home-assistant.io/integrations/template/)** - used for attribute extraction and calculations 🖌
- **[moon](https://www.home-assistant.io/integrations/moon/)** - used for get information about the current moon phase 🌜
- **[darksky](https://www.home-assistant.io/integrations/darksky/)** - used to get detailed weather information 🌦
- **[systemmonitor](https://www.home-assistant.io/integrations/systemmonitor/)** - used to get information about the host machine 🖥
- **[time](https://www.home-assistant.io/integrations/time_date/)** - used to get the current time as a sensor 🕖
- **[dwd_weather_warnings](https://www.home-assistant.io/integrations/dwd_weather_warnings/)** - used to get weather warnings ⚡️

## bed_weight.yaml ##

As decribed *here* im using [HX711](https://www.amazon.de/Menschlichen-Gewichtungssensor-Verstärker-Dehnungsmessgerät-Badezimmerwaage/dp/B07FMN1DBN/ref=sr_1_1_sspa?dchild=1&keywords=HX711&qid=1605812031&sr=8-1-spons&psc=1&spLa=ZW5jcnlwdGVkUXVhbGlmaWVyPUE5TFIxMEZBSU1BWEomZW5jcnlwdGVkSWQ9QTA4NTUxOTdHRjVFVFozRDZBUTcmZW5jcnlwdGVkQWRJZD1BMDIyMTYwNzJYV1JHRVZNUDhEMEQmd2lkZ2V0TmFtZT1zcF9hdGYmYWN0aW9uPWNsaWNrUmVkaXJlY3QmZG9Ob3RMb2dDbGljaz10cnVl)-Sensors to monitor the current weight laying in bed. As our bed has 8 feet I need two sensors, which values need to be added to a total weight.

This and the case distinction is handled in this file. A good explination and tutorial on this can be read [here](https://selfhostedhome.com/diy-bed-presence-detection-home-assistant/).

## days_until.yaml ##

In this file I'm creating template sensors which display a countdown to a specific date, at the moment there is only christmas. This information is displayed as random fact on the led_sign.

## garbage_collection.yaml ##

I've got an calender for garbage collection events only. The problem with these sensors is, that the next event is always present no matter how far its away. To work around this I created a sensor, that show 'true' if one of those garbage events is is on the next day.

## home_count.yaml ##

This sensor show the percentage of all residents that are home. It is mainly to do not trigger unnecessary ["monitor"](https://github.com/andrewjfreyer/monitor) scans. The source of this sensor can be found [here](https://github.com/DubhAd/Home-AssistantConfig/blob/live/sensors/home_count.yaml).

## opentherm.yaml ##

This sensors extracts the current "set"-temperature from my HVAC. It does not work at the moment...

## vacuum.yaml ##

This sensor extracts the battery status from my vacuum robot.