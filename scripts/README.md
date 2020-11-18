# Scripts #

In this folder, all of my scripts are located. I use then whenever I implement repetitive action sequences. Every file may contain multiple scripts, which are related to each other. In the following listing I briefly discribe each file.

## global_lighting.yaml ##

As I love my LED Strips, I love give use them with random colors and effects. The main thought is to give the apartment every evening a new vibe by setting a random color on all "ambient lights". There is also a script for a random effect on each compatible [WLED](https://github.com/Aircoookie/WLED)-Strip, but it is only just for fun.

## led_sign.yaml ##

Our LED-Sign has three states: "Default", "Hard" and "Notification", but "Notification" is based on "Hard". Every state has it's own script, which enabled displays the corresponding message (or random event) with the corresponding state.

## living_room_media.yaml ##

In our living_room are a lot of different devices, which are interacting with each other. We've got the lights, TV, AVR, PC, Wii and our PS4. The main controller in this room is a [WXKG02LM](https://de.aliexpress.com/item/32877238808.html?spm=a2g0o.productlist.0.0.2dc2610ao1Eubk&algo_pvid=5b3e3fd7-8bba-4599-a858-d2bba7fc7b57&algo_expid=5b3e3fd7-8bba-4599-a858-d2bba7fc7b57-2&btsid=0b0a182b16053946613325014e01f2&ws_ab_test=searchweb0_0,searchweb201602_,searchweb201603_), which executes scripts from this file. Each script represents an preset for all devices, configured for one specific use.

- Bright Lights
- Watch Netflix
- Play Wii
- Play PS4
- Play PC

## monitor.yaml ##

Contains all scripts corresponding to [monitor](https://github.com/andrewjfreyer/monitor). The idea behind the scanning pattern is [here](https://github.com/DubhAd/Home-AssistantConfig/tree/live/scripts).

## speech_engine.yaml and speech_processing.yaml ##

The main components of my speak assistant. If no specific media_player is set for audio playback, every single one is used, when he is not already in use. Thats because media played by TTS is treaten as a file, which implies that no interrupted music cannot be resumed. The main source for this [here](https://github.com/CCOSTAN/Home-AssistantConfig).

## vacuum.yaml ##

All complex commands which give the vacuum an task. By now there are only specific room-clearing tasks and driving to the bin.