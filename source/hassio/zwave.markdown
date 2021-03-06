---
layout: page
title: "Z-Wave"
description: "Instructions on how-to use Z-Wave with Hass.io."
date: 2017-04-30 13:28
sidebar: true
comments: false
sharing: true
footer: true
---

To enable Z-Wave, plug your Z-Wave USB stick into your Raspberry Pi 3 and add the following to your `configuration.yaml`:

```yaml
zwave:
  usb_path: /dev/ttyACM0
```

If you need GPIO on raspberry-pi3 for you Z-Wave module add follow line into `config.txt`:
```
dtoverlay=pi3-miniuart-bt
```

HUSBZB-1:
```yaml
zwave:
  usb_path: /dev/ttyUSB0
  
zha:
  usb_path: /dev/ttyUSB1
  database_path: /config/zigbee.db
```
