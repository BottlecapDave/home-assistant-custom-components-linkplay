# Linkplay Sound Devices integration v2

This component allows you to integrate control of audio devices based on Linkplay chipset into your [Home-Assistant](http://www.home-assistant.io) smart home system. Originally developed by nicjo814, maintained by limych. This version mostly rewritten by nagyrobi. Read more about Linkplay at the bottom of this file.

Fully compatible with [Mini Media Player card for Lovelace UI](https://github.com/kalkih/mini-media-player) by kalkih, including speaker group management.

### Warning !!!
This **will overwrite** the previous **Linkplay Sound Devices Integration** component if you had it installed. Also the configuration settings are not backwards compatible so **you will have to adjust** them as documented below otherwise it may break your system. To avoid this, make a backup of your previous linkplay config and remove it from your Home Assistant instance. Also uninstall/delete the previous linkplay component and restart Home Assistant.

[Configuration details and documentation](https://github.com/nagyrobi/home-assistant-custom-components-linkplay)

[Support forum](https://community.home-assistant.io/t/linkplay-integration/33878/133)

## Supported features:
- Configurable input sources list, to match choices in HA with the pyhsical inputs available on each device
- Configurable Icecast / Shoutcast webradio streams as input sources
- Retrieval of current playing content metadata from Icecast / Shoutcast webradio streams and filenames on directly attached USB sticks
- Retrieval of coverart from last.fm service based on current playing content metadata
- Multirooom in both WiFi-Direct and Router mode, using standard 'join' and 'unjoin' service calls.
- Recall of music presets stored on the device
- Snapshot and restore state of the player for smooth usage with TTS
- Browsing and playing media files from the directly attached USB sticks through Lovelace UI
- Linkplay-chipset specific commands through HA service calls

## About Linkplay

Linkplay is a smart audio chipset and module manufacturer. Their various module types share the same functionality across the whole platform and alow for native audio content playback from lots of sources, including local inputs, local files, Bluetooth, DNLA, Airplay and also web-based services like Icecast, Spotify, Tune-In, Deezer, Tidal etc. They allow setting up multiroom listening environments using either self-created wireless connections or relying on existing network infrastructure, for longer distances coverage. For more information visit https://linkplay.com/.
There are quite a few manufacturers and devices that operate on the basis of Linkplay platform. For more information check out the [documentation](https://github.com/nagyrobi/home-assistant-custom-components-linkplay#about-linkplay)

## Component authors & contributors
    "@nicjo814",
    "@limych",
    "@nagyrobi"
