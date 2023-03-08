# ESP32 Deauther

(Maybe) Port of https://github.com/spacehuhn/esp8266_deauther to the ESP32,
based on the `esp_wifi_80211_tx` function described in https://github.com/Jeija/esp32-80211-tx

# Building

Install [esp-idf](https://github.com/espressif/esp-idf). This project is built and tested with
commit 5ef1b390026270503634ac3ec9f1ec2e364e23b2.

`make` #Project has custom linker flags, run this instead of `idf.py build`

Built with v4.1-dev-763-ga45e99853

# Flashing

`make flash`


if for some reason you get this error "Desktop/esp32-deauther/main/main.cpp: In function 'void app_main()':
Desktop/esp32-deauther-master/main/main.cpp:44:5: error: 'tcpip_adapter_init' was not declared in this scope
   44 | tcpip_adapter_init();`" from main.cpp file

   just replace line 44 tcpip_adapter_init(); by tcpip_adapter_init();
