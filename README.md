# knot_P trackpad for ZMK firmware

## Build localy with devcontainer

In ZMK/app,

### Debug

```bash
west build -p --board seeeduino_xiao_ble -S zmk-usb-logging  -- -DSHIELD=knot_p -DZMK_CONFIG="/workspaces/zmk-config" -DZMK_EXTRA_MODULES="/workspaces/zmk-modules/cirque-input-module;/workspaces/zmk-modules/zmk-input-gestures;/workspaces/zmk-modules/zmk-input-processors/"
```

### Release

```bash
west build -p --board seeeduino_xiao_ble -- -DSHIELD=knot_p -DZMK_CONFIG="/workspaces/zmk-config" -DZMK_EXTRA_MODULES="/workspaces/zmk-modules/cirque-input-module;/workspaces/zmk-modules/zmk-input-gestures;/workspaces/zmk-modules/zmk-input-processors/"
```
