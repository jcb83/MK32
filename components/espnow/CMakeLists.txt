set(COMPONENT_SRCS "espnow_recieve.c"
    "espnow_send.c")
set(COMPONENT_ADD_INCLUDEDIRS ".")
set(COMPONENT_REQUIRES ble_new esp_wifi nvs_flash r_encoder)

register_component()
