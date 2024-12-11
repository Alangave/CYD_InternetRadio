
board :
      "'-D TFT_WIDTH=240'",
      "'-D TFT_HEIGHT=320'",

platformio.ini :

[platformio]
default_envs = esp32-2432S028R

[env]
platform = espressif32
framework = arduino
monitor_speed = 115200
lib_deps = lovyan03/LovyanGFX@^1.2.0
	https://github.com/pschatzmann/arduino-audio-tools
	https://github.com/pschatzmann/arduino-libhelix.git
build_flags = 
	-DCORE_DEBUG_LEVEL=3


CYD_InternetRadio/lib/lgfx_ESP32_2432S028/lgfx_ESP32_2432S028.h
Panel:
      cfg.offset_rotation  = 0;             // offset of rotation direction value 0~7 (4~7 is upside down)

      cfg.invert     = true;        

touch :
      cfg.offset_rotation = 6;