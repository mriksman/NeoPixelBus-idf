idf_component_register(
    SRCS
        "neopixelbus/src/internal/HsbColor.cpp"
        "neopixelbus/src/internal/HslColor.cpp"
        "neopixelbus/src/internal/HtmlColor.cpp"
        "neopixelbus/src/internal/HtmlColorNames.cpp"
        "neopixelbus/src/internal/HtmlColorNameStrings.cpp"
        "neopixelbus/src/internal/HtmlColorShortNames.cpp"
        "neopixelbus/src/internal/NeoEsp32RmtMethod.cpp"
        "neopixelbus/src/internal/NeoGamma.cpp"
        "neopixelbus/src/internal/NeoPixelAnimator.cpp"
        "neopixelbus/src/internal/Rgb48Color.cpp"
        "neopixelbus/src/internal/RgbColor.cpp"
        "neopixelbus/src/internal/RgbColorBase.cpp"
        "neopixelbus/src/internal/RgbwColor.cpp"
        "neopixelbus/src/internal/SegmentDigit.cpp"
    INCLUDE_DIRS .
)

target_compile_definitions(${COMPONENT_TARGET} PRIVATE 
    "-DARDUINO_ARCH_ESP32")