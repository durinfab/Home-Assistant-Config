# A whole lotta automations ⚙️ #

This entire folder is included into the ["automation"-integration](https://www.home-assistant.io/integrations/automation/). Each file and folder is briefly described here. 

## initial_states.yaml ##

This file handles all automations regarding the start and shutdown of home assistant.

## 🚨 alarm_management/ ##

Covers all automations regarding the security system. At the I'm using a single [alarm_control_panel](https://www.home-assistant.io/integrations/alarm_control_panel/) entity to represent the state of my house. Here are described how these are getting enabled and disabled.

## 🔋 battery/ ##

As I'm using a lot battery powered devices, I need to monitor their state to avoid a device dieing. These are devided into different battery-types to send a fitting notification. The Source of this idea is [here](https://github.com/DubhAd/Home-AssistantConfig/tree/live/automation/battery).

## 🚦 debugpanel/ ##

My debugpanel features 12 LEDs, two switches and one PIR-Sensor. Every component got it's own automation file. The LEDs are labeled by the position in their array, because I usually change their purpose.

## 🌇 evening_routine/ ##

A lot of lighting automations are enabled and events are fired in the evening. That's why this state is represented by it's own [input_boolean](https://www.home-assistant.io/integrations/input_boolean/).

## 🔥 hvac/ ##

This folder contains all automations regarding the HVAC. I use an [OpenTherm Gateway](https://www.nodo-shop.nl/nl/opentherm-gateway/188-opentherm-gateway.html) to communicate with my heater. Looking forward to [this](https://github.com/rvdbreemen/OTGW-firmware) to get released. 

## 🎉 miscellaneous/ ##

This folder contains all automations with no matching category. Some of them are oly just for fun.

## 🏠 presence/ ##

This folder contains all automations regarding the presence detection with the [Nmap-Integration](https://www.home-assistant.io/integrations/nmap_tracker/) and ["monitor"](https://github.com/andrewjfreyer/monitor).

## 🪴 rooms/ ##

Room specific automations are devided to their corresponding area. Mainly for a personal overview.

## 📱 tablet/ ##

My wall mounted Fire Tablet is involved in some automations. These are stored here.

## 🧹 vacuum/ ##

All automations regarding my vacuum robot contained in the folder.