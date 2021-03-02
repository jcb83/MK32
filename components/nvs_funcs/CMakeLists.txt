set(COMPONENT_SRCS "arr_conv.c"
    "nvs_funcs.c")
set(COMPONENT_ADD_INCLUDEDIRS ".")
set(COMPONENT_PRIV_INCLUDEDIRS "../../main")
set(COMPONENT_REQUIRES nvs_flash u8g2_OLED)

register_component()
