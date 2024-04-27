# KioskDisplayControl
this collection of scrips are meant to configure and control a raspberry pi based wall display.

I'm using this for a home assistant dashboard, but with small changes it should be suitable for other applications.

## architecture 
I'm using mqtt for sending control commands. You can set up this as homeassistant add-on.

## hardware 
you need at least 

- a raspberry pi (at least a zero2w)
- a high performance SD card (a slow SD card was a huge issue for me)
- a good power supply
- a display (you can use the official display. I'm using the waveshare Zero-DISP-7A)

## setup 
follow the official instructions for installation of rasbian. I recommend to preset WiFi, hostname, user and ssh before installing.

- Clone this repo into the home directory.
- rename config.example to config
- run install
  - install dependencies
  - setup autostart
    - start mqtt-listener
    - start browser in kiosk mode 
