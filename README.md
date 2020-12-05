# Home Assistant Configuration

## Setup

I'm running Home Assistant using this: https://community.home-assistant.io/t/hass-io-on-synology-dsm-native-package/125559/2 (I added SynoCommunity to my packages, and then you can find the package, which will start up a bunch of dockers).

I bought this Zigbee bridge: https://phoscon.de/en/conbee2, which is connected to the Synology (using an USB extenstion cord for better reception)

I'm running it with https://github.com/marthoc/docker-deconz running on the Synology in a Docker.

## HomeKit

I'm treating Home Assistant as the source for all things smart, and I'm exposing most things from Home Assistant to HomeKit, this way there is an nice builtin interface for quickly turning off/on a light.

A side effect of buying things 'Designed for HomeKit' is that the device will work without an external server, also a win.

## Rules

- Don't be too smart
- Expect to keep working without internet
- Nothing essential (only scenic lights etc)
