# U-boot 2022.10 Patches

Baseline: <https://github.com/u-boot/u-boot/tree/v2022.10>

Official Modified U-boot Source: <https://github.com/DasSecurity-HatLab/u-boot-2022.10-gateboard-one>

## Apply Patches

```bash
git clone --branch=v2022.10 https://github.com/u-boot/u-boot.git --depth 1
cd u-boot

# apply patch
git apply patches/uboot/2022.10/0001-add-hatlab-gateboard-one.patch

# make build
make
```
