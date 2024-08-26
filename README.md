# Example configuration
```
external_components:
  - source:
      type: git
      url: https://github.com/markv9401/esphome_gree_hvac
      ref: dev
    components: [ gree ]
    refresh: 0s

uart:
  id: ac_uart
  tx_pin: GPIO1
  rx_pin: GPIO3
  baud_rate: 4800
  data_bits: 8
  parity: EVEN
  stop_bits: 1

climate:
  - platform: gree
    name: GreeHVAC_Bedroom
    supported_presets:
      - "NONE"
      - "BOOST"
      - "SLEEP"
    supported_swing_modes:
      - "VERTICAL"
      - "HORIZONTAL"
      - "BOTH"
      - "OFF"
```
