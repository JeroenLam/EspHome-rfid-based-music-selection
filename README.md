# RFID based virtual music library

The goal of this project is to create a ESPHome based RFID reader that can be used to automatically trigger events in Home Assistant. With the subgoal to have a physical system that can be used to turn on and switch between multiple music playlists, similar to CD's.

## Hardware
- ESP32 dev board or ESP8266 D1 mini
- RC522 RFID reader
- 3 buttons
- 3d printed case (files included for D1 mini)
- Wires
- Heatset m5 inserts
- m5 screws
- Soldering iron

Fotos of the building process are included at the bottom of the README.

## Wiring 
![Wiring diagram of project](./assets/circuit_image.svg)

# What is implemented
- Minimal working hardware demo for RFID tags being placed on and being removed from the sensor
- Blueprint that can be used to easily link tags to (Spotify) playlists
- Shuffle the target playlists
- Joining multiple audio sources automatically from the blueprint
- Media controlls on the esp device

## Media control
- Left (single press): Previous song
- Right (signle press): Next song
- Middle: Play/Pause
- Left (hold): Volume down
- Right (hold): Volume up

# What is being worked on
- Support for other audio sources
- 3d printable cartridges for the music
- Guidlines on tags that are supported
- Environmental sensors that can be added to the device

# Assembly images
![Dev board esp32](/assets/1_esp32_example.jpg)

The example below is with the ESP8266 D1 mini

![Wiring RFID reader](/assets/2_wiring_rfid_reader.jpg)
![Wiring Buttons](/assets/3_wiring_buttons.jpg)
![Fitting buttons in case](/assets/4_fitting_buttons_in_case.jpg)
![Fitting all wires in case](/assets/5_fitting_everything_in_case.jpg)
Stuff all wires under the overhang of the rfid board to keep them compacted.
![How it should look before closing the lid](/assets/6_fitting_everything_in_case_before_cover.jpg)
![Final assembly](/assets/7_final.jpg)

