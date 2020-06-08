# NeoPixelBus-idf
NeoPixelBus with Support for ESP-IDF

How to get https://github.com/Makuna/NeoPixelBus working with ESP-IDF

Review the files in this repo;
* `NeoEsp32RmtMethod.h` is a copy of the one on NeoPixelBus, except the `ifdef` is changed.
* `NeoPixelAnimator.h` is a copy of the one on NeoPixelBus, except the `include` is changed.
* `NeoPixelBrightnessBus.h` and `NeoPixelSegmentBus.h` are exact copies. You can't use the ones in the main NeoPixelBus library, because they include `NeoPixelBus.h` which includes files which do not work with ESP-IDF.
* `NeoPixelBus.h` is a copy of the one on NeoPixelBus, except the `includes` are changed. This only supports ESP32 with RMT.
* `Arduino.h` are the missing Arduino pieces.
     
