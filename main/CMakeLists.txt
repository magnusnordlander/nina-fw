set(inc_dir "."
            "../components/arduino-core-esp32"
            "../components/libraries"
)

if(NOT CMAKE_BUILD_EARLY_EXPANSION) 
	add_definitions(-DARDUINO)
endif() 


idf_component_register(SRCS "main.cpp" "sketch.ino.cpp" "http_client.c" "ECCX08Cert.cpp" "CryptoUtil.cpp" "CommandHandler.cpp"
                    INCLUDE_DIRS "${inc_dir}")