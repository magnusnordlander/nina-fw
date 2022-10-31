idf_component_register(SRC_DIRS
                    "ArduinoBearSSL/src"
                    "ArduinoBearSSL/src/bearssl"
                    "ArduinoBearSSL/src/utility"
                    "SPIS/src"
                    "WiFi/src"
                    "Wire/src"
                    "ArduinoECCX08/src"
                       INCLUDE_DIRS 
                    "ArduinoBearSSL/src"
                    "SPIS/src"
                    "WiFi/src"
                    "Wire/src"
                    "ArduinoECCX08/src"
                       REQUIRES arduino-core-esp32 wpa_supplicant xtensa lwip)

if(NOT CMAKE_BUILD_EARLY_EXPANSION) 
    add_definitions(-DARDUINO)
endif() 