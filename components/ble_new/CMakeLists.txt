set(COMPONENT_SRCS "hal_ble.c"
                   "hid_dev.c"
                   "hid_device_le_prf.c"
                   "keyboard.c")
set(COMPONENT_ADD_INCLUDEDIRS "." "../../main")
set(COMPONENT_REQUIRES bt u8g2_OLED)

register_component()

if(GCC_NOT_5_2_0)
    component_compile_options(-Wno-unused-const-variable)
endif()
