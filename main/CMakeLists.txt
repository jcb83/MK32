set(srcs "."
    "../plugins"
    "../plugins/plugin_components/hid_keycode_conv"
    "../plugins/plugin_components/wifi_manager"
    "../plugins/plugin_components"
    "../components/nvs_funcs"
    "../components/battery_monitor"
    "../components/u8g2_OLED"
    "../components/r_encoder"
    "../components/espnow"
    "../components/ble_new"
)

set(includes "."
    "../plugins"
    "../plugins/plugin_components/hid_keycode_conv"
    "../plugins/plugin_components/wifi_manager"
    "../plugins/plugin_components"
    "../components/nvs_funcs"
    "../components/battery_monitor"
    "../components/u8g2_OLED"
    "../components/r_encoder"
    "../components/espnow"
    "../components/ble_new" 
)

idf_component_register(
    SRC_DIRS "${srcs}"
    INCLUDE_DIRS "${includes}"
    REQUIRES bt json u8g2_OLED
    EMBED_TXTFILES ../plugins/cacert.pem ../plugins/prvtkey.pem
)