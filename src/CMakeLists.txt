add_library(driver_cd74hc595 cd74hc595.cc cd74hc595.h cd74hc595.pio.h)
target_link_libraries(driver_cd74hc595 PRIVATE hardware_gpio hardware_pio hardware_clocks)
pico_generate_pio_header(driver_cd74hc595 ${CMAKE_CURRENT_LIST_DIR}/cd74hc595.pio)
