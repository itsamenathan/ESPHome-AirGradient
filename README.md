# ESPHome-AirGradient

ESPHome config for AirGradient Air Quality Sensor

Forked from: <https://github.com/ajfriesen/ESPHome-AirGradient>

The AirGradient DIY Air Quality Sensor can be found here: <https://www.airgradient.com/diy/>

This repository will provide you the ESPHome config to run this with Home Assistant.

## Prerequisites

* You need to have [Home Assistant](https://www.home-assistant.io/installation/) running
* You will also need the ESPHome Add-on. [Open ESPHome Add-on](https://my.home-assistant.io/redirect/supervisor_addon/?addon=a0d7b954_esphome) in Home Assistant.

## Add your secrets

* Rename `secrets-default.yaml` to `secrets.yaml`
* Update the contents `secrets.yaml` file

## Upload Firmware

``` bash
# Compile
esphome compile air-gradient-diy.yaml

# Flash
esphome upload air-gradient-diy.yaml
```

## Adpot in Home Assistant

* Go to Home Assistant
* A new device should be ready to configure
* You will need to provide the encryption key from your `secrets.yaml` file
