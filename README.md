# RF24 – ESP32 (ESP-IDF) adaptation

This repository is the [RF24](https://github.com/nRF24/RF24) library **adapted for ESP32 (ESP-IDF)**. It provides the NRF24L01 driver as an ESP-IDF component.

- **Used by:** [project-esp32-embedsyst-cpp_ble-jammer-nrf24l01](https://github.com/AntonBronnfjell/project-esp32-embedsyst-cpp_ble-jammer-nrf24l01) (included as a submodule).
- **Original:** [nRF24/RF24](https://github.com/nRF24/RF24).

## ESP-IDF integration

- Component name: **RF24** (use `REQUIRES RF24` in your app’s `CMakeLists.txt`).
- ESP-IDF-specific code lives in **utility/esp_idf/** (SPI, GPIO, compatibility, interrupts). The root `CMakeLists.txt` registers the component with `idf_component_register`.
