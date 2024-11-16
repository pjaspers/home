# Home Assistant Configuration

## Setup

I used to run this on a Synology using this: https://community.home-assistant.io/t/hass-io-on-synology-dsm-native-package/125559/2, but have now switched to match the Home Assistant blessed hardware (and it is so much faster):

- ODROID-N2+
- 64gb eMMC

I bought this Zigbee bridge: https://phoscon.de/en/conbee2, which is connected to the odroid (using an USB extension cord for better reception), and using the Deconz addon



## HomeKit

I'm treating Home Assistant as the source for all things smart, and I'm exposing most things from Home Assistant to HomeKit, this way there is an nice builtin interface for quickly turning off/on a light.

A side effect of buying things 'Designed for HomeKit' is that the device will work without an external server, also a win.

## Rules

- Don't be too smart
- Expect to keep working without internet
- Nothing essential (only scenic lights etc)

House will go to sleep at: {{ states.input_datetime.go_to_bed_house.attributes.hour }}:{{ states.input_datetime.go_to_bed_house.attributes.minute }}

Girls will wake up at: {{ states.input_datetime.alarm_clock_girls.attributes.hour }}:{{ states.input_datetime.alarm_clock_girls.attributes.minute }}
