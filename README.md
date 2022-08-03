# task 2 ESP-Watson-
Connect the ESP to my laptop and phone using Arduino

***

ESP Watson 32


The physical connection


Connect the USB to micro USB cable from the ESP to the laptop via the micro via USB and make sure the turn signal lights on the ESP are on, if the laptop isn't connected it should show a notification on the laptop. Proceed to the next step, I will explain the problem and how to fix it, skip the next step


If the port is not visible
After connecting the ESP to the USB port, the laptop may not recognize the device to configure it with Arduino (which we will cover in the next step). To fix this we go to your OS settings via windows button is it windows 10 then search on this page in the top right corner (about your pc) you will find the device manager see Universal Serial Bus Control Right click on port with yellow exclamation mark and update driver manually and search for driver in google and download from https://www.silabs.com/developers/usb-to-uart-bridge-vcp-drivers and put path In the update driver section it appears everywhere, even on Arduino


Set up Arduino


Download Arduino from https://www.arduino.cc/en/software. Choose the correct link based on your system. It's just an IDE that connects to the robot and uses C-based scripts.

Customize ESP 32 on Arduino
In order for the Arduino to recognize the ESP 32, you need to select Tools > Board > Board Manager > then search for ESP 32 and click Install. It's actually a package that allows you to control the ESP

After that you have to do another step from File > Settings > next to the other board manager urls: to include them https://dl.espressif.com/dl/package_esp32_index.json

startup script
There is a simple code example available in Arduino. In our task we want to make sure the ESP32 is working and since it has an LED we want the LED to blink at different frequencies, do this from File > Examples > Basic > Blinking. When you write the speed in milliseconds, start code that turns the flash on and off at different frequencies.
