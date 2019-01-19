# Roku TV Custom Driver for Hubitat

## Introduction

This is a fork of the SmartThings Device Handler found here: [ericboehs/smartthings-roku-tv](https://github.com/ericboehs/smartthings-roku-tv)

It allows you to send basic commands such as on/off, volume, and inputs to a Roku TV.

![Commands](/Screenshots/commands.PNG?raw=true)

## Configuration

When adding the device, you'll need to specify the "Device Network Id" in Hubitat. The Device Network ID is the IP and port of your TV in hex. miniwebtool has good [IP to Hex Converter](http://www.miniwebtool.com/ip-address-to-hex-converter/) you can use. It doesn't do port but the default port of `8060` is `1F7C` in hex. For example, if your IP was 10.0.1.15, your Device Network Id would be `0A00010F:1F7C` (note the leading 0).

![Device Information](/Screenshots/device_information.PNG?raw=true)

You'll also need to configure the Device IP and MAC Address in the preferences. The MAC address shouldn't contain any delimiters such as spaces or colons. For example a MAC address of `BA:F1:2E:DC:34:2A` should be entered as `BAF12EDC342A`.

![Preferences](/Screenshots/preferences.PNG?raw=true)

A fancier Device Type would handle all this for you. I'm sorry I haven't taken the time for that. I welcome Pull Requests that implement this feature.

## Issues
Please report issues via GitHub Issues.

## License
MIT License. See [License](https://github.com/ericboehs/smartthings-roku-tv/LICENSE).
