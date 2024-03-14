Prebuilt MIUI Camera to include in custom ROM builds.

Reference: https://github.com/Tree-sources/vendor_xiaomi-sweet-miuicamera

### Supported device
* Redmi Note 10s (Rosemary)

### How to use?

1. Clone this repo to `vendor/xiaomi/rosemary-miuicamera`

2. Inherit it from `device.mk` in device tree:

```
# Camera
$(call inherit-product-if-exists, vendor/xiaomi/rosemary-miuicamera/products/miuicamera.mk)
```

3. Include sepolicy to `BoardConfig.mk` in device tree:

```
# Sepolicy
include vendor/xiaomi/rosemary-miuicamera/products/board.mk
```
