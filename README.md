Word Clock based on Wemos D1 mini / ESP8266
===========================================

Required board support
----------------------
add http://arduino.esp8266.com/versions/2.4.0/package_esp8266com_index.json as additional board manager URL

Required libraries
------------------
- Adafruid NeoPixel
- Time
- ArduinoJson
- WiFiManager
- https://github.com/ratkins/RGBConverter

Features
--------

- LEDs
  - Control of WS2812B LED strip
  - Ambilight
  - Color in HSV
  - Brightness adjusted by LDR

- Time
  - Obtained by NTP
  - Wifimanager used to connect to Wifi

- Webserver:
  - All parameters can be set with simple web server
  - Access to web server: Type wordclock.local in your browser

- Night-time:
  - Word clock LEDs can be switched off at night
  - Start and end time can be set manually

- Others
  - Language: German/English
  - Display of current date

Wiring
------

- LED IDs:
  - Rows from top to bottom:
  - 1-11
  - 22-12
  - 23-33
  - 44-34
  - 45-55
  - 66-56
  - 67-77
  - 88-78
  - 89-99
  - 110-100
  - LEDs for single minutes: 111-114
  - All remaining LEDs belong to ambilight

- LDR:
  - 3.3V —— LDR —— A0 —— 10k —— GND
