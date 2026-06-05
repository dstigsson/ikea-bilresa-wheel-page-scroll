Create this helper first in Home Assistant:

input_number:
  bilresa_last_action_level:
    name: Bilresa Last Action Level
    min: 0
    max: 255
    step: 1

Replace these two in "ikea-bilresa-wheel-page-scroll.yaml":
zigbee2mqtt/YOUR_BILRESA_NAME
select.YOUR_ESPHOME_SCREEN_SELECTOR

Example:
topic: zigbee2mqtt/bilresa_remote
screen_selector: select.eink_screen_selector
