set(COMPONENT_SRCS "battery_monitor.c")
set(COMPONENT_ADD_INCLUDEDIRS ".")
set(COMPONENT_PRIV_INCLUDEDIRS "../../main")
set(COMPONENT_REQUIRES esp_adc_cal u8g2_OLED)

register_component()
