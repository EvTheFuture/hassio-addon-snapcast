# Snapcast add-on for Home Assistant

This add-on allow you to have a snapcast server and/or client running on Home Assistant to get synchronius audio in multiple rooms.

[Snapcast](https://github.com/badaix/snapcast) is a multiroom client-server audio player developed by [badaix](https://github.com/badaix), where all clients are time synchronized with the server to play perfectly synced audio. It's not a standalone player, but an extension that turns your existing audio player into a Sonos-like multiroom solution.

[Read more about Snapcast here](https://github.com/badaix/snapcast)

## Features
Currently only the librespot stream is implemented in this add-on which provide synchronius playback for Spotify on multiple devices.

## Installation
* In the Home Assistant Add-on store, add the repository: https://github.com/EvTheFuture/hassio-addon-repository
* Search for Snapcast and install the Add-on

## Configuration
The following configuration options exists

### Server
- `enable`: true|false (Shall the snapcast server be enabled or not)
- `enable_web`: true|false (Shall the web interface be enabled or not)
- `enable_stream_librespot`: true|false (Shall spotify be enabled or not)
- `librespot_name:` The name of the spotify service
- `librespot_device_name`: The name to present in spotify connect
- `librespot_initial_volume`: Initial volume in (0-100)%
- `librespot_bitrate`: Bitrate (96|160|320)
- `librespot_normalize`: true|false (Use spotify's normalization or not)
- `librespot_killall`: true|false 
- `librespot_disable_audio_cache`: true|false
- `librespot_params`: Any extra parameters for this stream.
- `librespot_extra_params`: Any extra parameters to send to librespot.

### Client
- `enable`: true|false (Shall the snapcast client be enabled or not)
- `host`: address to the snapcast server
- `extra_params`: Any extra parameters to use when startign the client process.

## Support my work
[![buy-me-a-coffee](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/EvTheFuture)
