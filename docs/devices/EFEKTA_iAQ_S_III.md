---
title: "EFEKTA EFEKTA_iAQ_S_III control via MQTT"
description: "Integrate your EFEKTA EFEKTA_iAQ_S_III via Zigbee2MQTT with whatever smart home infrastructure you are using without the vendor's bridge or gateway."
addedAt: 2025-04-01T18:30:52
pageClass: device-page
---

<!-- !!!! -->
<!-- ATTENTION: This file is auto-generated through docgen! -->
<!-- You can only edit the "Notes"-Section between the two comment lines "Notes BEGIN" and "Notes END". -->
<!-- Do not use h1 or h2 heading within "## Notes"-Section. -->
<!-- !!!! -->

# EFEKTA EFEKTA_iAQ_S_III

|     |     |
|-----|-----|
| Model | EFEKTA_iAQ_S_III  |
| Vendor  | [EFEKTA](/supported-devices/#v=EFEKTA)  |
| Description | Air Quality Monitor, CO2, VOC, outdoor temperature and humidity, date and time |
| Exposes | co2, voc_index, temperature, humidity, illuminance, auto_brightness, night_onoff_backlight, night_on_backlight, night_off_backlight, long_chart_period, long_chart_period2, internal_or_external, temperature_offset, humidity_offset, set_altitude, automatic_scal, forced_recalibration, factory_reset_co2, manual_forced_recalibration, enable_co2, invert_logic_co2, high_co2, low_co2, enable_voc, invert_logic_voc, high_voc, low_voc |
| Picture | ![EFEKTA EFEKTA_iAQ_S_III](https://www.zigbee2mqtt.io/images/devices/EFEKTA_iAQ_S_III.png) |


<!-- Notes BEGIN: You can edit here. Add "## Notes" headline if not already present. -->


<!-- Notes END: Do not edit below this line -->



## Options
*[How to use device type specific configuration](../guide/configuration/devices-groups.md#specific-device-options)*

* `co2_calibration`: Calibrates the co2 value (absolute offset), takes into effect on next report of device. The value must be a number.

* `temperature_calibration`: Calibrates the temperature value (absolute offset), takes into effect on next report of device. The value must be a number.

* `temperature_precision`: Number of digits after decimal point for temperature, takes into effect on next report of device. This option can only decrease the precision, not increase it. The value must be a number with a minimum value of `0` and with a with a maximum value of `3`

* `humidity_calibration`: Calibrates the humidity value (absolute offset), takes into effect on next report of device. The value must be a number.

* `humidity_precision`: Number of digits after decimal point for humidity, takes into effect on next report of device. This option can only decrease the precision, not increase it. The value must be a number with a minimum value of `0` and with a with a maximum value of `3`

* `illuminance_calibration`: Calibrates the illuminance value (percentual offset), takes into effect on next report of device. The value must be a number.

* `illuminance_raw`: Expose the raw illuminance value. The value must be `true` or `false`


## Exposes

### CO2 (numeric)
Measured value.
Value can be found in the published state on the `co2` property.
It's not possible to read (`/get`) or write (`/set`) this value.
The unit of this value is `ppm`.

### Voc index (numeric)
VOC index.
Value can be found in the published state on the `voc_index` property.
It's not possible to read (`/get`) or write (`/set`) this value.
The unit of this value is `VOC Index points`.

### Temperature (numeric)
Measured temperature value.
Value can be found in the published state on the `temperature` property.
It's not possible to read (`/get`) or write (`/set`) this value.
The unit of this value is `°C`.

### Humidity (numeric)
Measured relative humidity.
Value can be found in the published state on the `humidity` property.
It's not possible to read (`/get`) or write (`/set`) this value.
The unit of this value is `%`.

### Illuminance (numeric)
Measured illuminance.
Value can be found in the published state on the `illuminance` property.
It's not possible to read (`/get`) or write (`/set`) this value.
The unit of this value is `lx`.

### Auto brightness (binary)
Enable or Disable Auto Brightness of the Display.
Value can be found in the published state on the `auto_brightness` property.
It's not possible to read (`/get`) this value.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"auto_brightness": NEW_VALUE}`.
If value equals `ON` auto brightness is ON, if `OFF` OFF.

### Night onoff backlight (binary)
Complete shutdown of the backlight at night mode.
Value can be found in the published state on the `night_onoff_backlight` property.
It's not possible to read (`/get`) this value.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"night_onoff_backlight": NEW_VALUE}`.
If value equals `ON` night onoff backlight is ON, if `OFF` OFF.

### Night on backlight (numeric)
Night mode activation time.
Value can be found in the published state on the `night_on_backlight` property.
It's not possible to read (`/get`) this value.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"night_on_backlight": NEW_VALUE}`.
The minimal value is `0` and the maximum value is `23`.
The unit of this value is `Hr`.

### Night off backlight (numeric)
Night mode deactivation time.
Value can be found in the published state on the `night_off_backlight` property.
It's not possible to read (`/get`) this value.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"night_off_backlight": NEW_VALUE}`.
The minimal value is `0` and the maximum value is `23`.
The unit of this value is `Hr`.

### Long chart period (enum)
The period of plotting the CO2 level(OFF - 1H | ON - 24H).
Value can be found in the published state on the `long_chart_period` property.
It's not possible to read (`/get`) this value.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"long_chart_period": NEW_VALUE}`.
The possible values are: `1H`, `24H`.

### Long chart period2 (enum)
The period of plotting the VOC Index points(OFF - 1H | ON - 24H).
Value can be found in the published state on the `long_chart_period2` property.
It's not possible to read (`/get`) this value.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"long_chart_period2": NEW_VALUE}`.
The possible values are: `1H`, `24H`.

### Internal or external (enum)
Display data from internal or external TH sensor.
Value can be found in the published state on the `internal_or_external` property.
It's not possible to read (`/get`) this value.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"internal_or_external": NEW_VALUE}`.
The possible values are: `INTERNAL`, `EXTERNAL`.

### Temperature offset (numeric)
Adjust temperature.
Value can be found in the published state on the `temperature_offset` property.
It's not possible to read (`/get`) this value.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"temperature_offset": NEW_VALUE}`.
The minimal value is `-50` and the maximum value is `50`.
The unit of this value is `°C`.

### Humidity offset (numeric)
Adjust humidity.
Value can be found in the published state on the `humidity_offset` property.
It's not possible to read (`/get`) this value.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"humidity_offset": NEW_VALUE}`.
The minimal value is `-50` and the maximum value is `50`.
The unit of this value is `%`.

### Set altitude (numeric)
Setting the altitude above sea level (for high accuracy of the CO2 sensor).
Value can be found in the published state on the `set_altitude` property.
It's not possible to read (`/get`) this value.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"set_altitude": NEW_VALUE}`.
The minimal value is `0` and the maximum value is `3000`.
The unit of this value is `meters`.

### Automatic scal (binary)
Automatic self calibration.
Value can be found in the published state on the `automatic_scal` property.
It's not possible to read (`/get`) this value.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"automatic_scal": NEW_VALUE}`.
If value equals `ON` automatic scal is ON, if `OFF` OFF.

### Forced recalibration (binary)
Start FRC (Perform Forced Recalibration of the CO2 Sensor).
Value can be found in the published state on the `forced_recalibration` property.
It's not possible to read (`/get`) this value.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"forced_recalibration": NEW_VALUE}`.
If value equals `ON` forced recalibration is ON, if `OFF` OFF.

### Factory reset co2 (binary)
Factory Reset CO2 sensor.
Value can be found in the published state on the `factory_reset_co2` property.
It's not possible to read (`/get`) this value.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"factory_reset_co2": NEW_VALUE}`.
If value equals `ON` factory reset co2 is ON, if `OFF` OFF.

### Manual forced recalibration (numeric)
Start Manual FRC (Perform Forced Recalibration of the CO2 Sensor).
Value can be found in the published state on the `manual_forced_recalibration` property.
It's not possible to read (`/get`) this value.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"manual_forced_recalibration": NEW_VALUE}`.
The minimal value is `0` and the maximum value is `5000`.
The unit of this value is `ppm`.

### Enable co2 (binary)
Enable CO2 Gas Control.
Value can be found in the published state on the `enable_co2` property.
It's not possible to read (`/get`) this value.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"enable_co2": NEW_VALUE}`.
If value equals `ON` enable co2 is ON, if `OFF` OFF.

### Invert logic co2 (binary)
Enable invert logic CO2 Gas Control.
Value can be found in the published state on the `invert_logic_co2` property.
It's not possible to read (`/get`) this value.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"invert_logic_co2": NEW_VALUE}`.
If value equals `ON` invert logic co2 is ON, if `OFF` OFF.

### High co2 (numeric)
Setting High CO2 Gas Border.
Value can be found in the published state on the `high_co2` property.
It's not possible to read (`/get`) this value.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"high_co2": NEW_VALUE}`.
The minimal value is `400` and the maximum value is `5000`.
The unit of this value is `ppm`.

### Low co2 (numeric)
Setting Low CO2 Gas Border.
Value can be found in the published state on the `low_co2` property.
It's not possible to read (`/get`) this value.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"low_co2": NEW_VALUE}`.
The minimal value is `400` and the maximum value is `5000`.
The unit of this value is `ppm`.

### Enable voc (binary)
Enable CO2 Gas Control.
Value can be found in the published state on the `enable_voc` property.
It's not possible to read (`/get`) this value.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"enable_voc": NEW_VALUE}`.
If value equals `ON` enable voc is ON, if `OFF` OFF.

### Invert logic voc (binary)
Enable invert logic CO2 Gas Control.
Value can be found in the published state on the `invert_logic_voc` property.
It's not possible to read (`/get`) this value.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"invert_logic_voc": NEW_VALUE}`.
If value equals `ON` invert logic voc is ON, if `OFF` OFF.

### High voc (numeric)
Setting High CO2 Gas Border.
Value can be found in the published state on the `high_voc` property.
It's not possible to read (`/get`) this value.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"high_voc": NEW_VALUE}`.
The minimal value is `0` and the maximum value is `500`.
The unit of this value is `ppm`.

### Low voc (numeric)
Setting Low CO2 Gas Border.
Value can be found in the published state on the `low_voc` property.
It's not possible to read (`/get`) this value.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"low_voc": NEW_VALUE}`.
The minimal value is `0` and the maximum value is `500`.
The unit of this value is `ppm`.

