# ZMK config for wireless Charybdis Nano 3x5 https://bastardkb.com/charybdis/

Build based on VOID's and EIGA's instructions from this video: https://www.youtube.com/watch?v=Mks7QDxFreY

Used nice!nano v2 controllers https://nicekeyboards.com/nice-nano

Plates modded by VOID:
- Elite-C adapter for nice!nano: https://github.com/victorlucachi/Elite-C-holder
- PMW3610 sensor breakout: https://github.com/victorlucachi/charybdis-pmw3610-breakout

VOID's zmk repo with mouse support and PMW3610 driver: 
https://github.com/victorlucachi/zmk/tree/pmw3610-aml

## Board config
Board config files are placed in `config/boards/shields/cnano` directory.

Trackball parameters are in `cnano_right.conf`. Most useful is `CONFIG_PMW3610_CPI=1600`, it sets sensor resolution.

## Keymap
Keymap is here: `config/cnano.keymap`

It was created with online zmk keymap editor: https://nickcoutsos.github.io/keymap-editor/, but after adding mouse layer config became not supported by editor :(

My layout is based on Miryoku https://github.com/manna-harbour/miryoku with home row, but has a lot of modifications to use Polish and Cyrillic letters and strongly remapped additional layers.

I would recommend to delete Mouse layer in `config/cnano.keymap`, make commit to repo and than edit keymap with online editor. Aftep that pull changes locally and add Mouse layer.

Or you can try to convert your QMK layout (if you have one) with online converter: https://github.com/aaronsantiago/qmk-to-zmk