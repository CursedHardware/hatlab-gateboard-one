# OpenWrt 21.02.5 Patches

Baseline: <https://github.com/openwrt/openwrt/tree/v21.02.5>

Official Modified OpenWrt source: <https://github.com/DasSecurity-HatLab/openwrt>

Pre-compiled firmware: <http://open.hatlab.dbappsecurity.com.cn/gateboard-one/repo/>

## Apply Patches

```bash
git clone --branch=v21.02.5 https://github.com/openwrt/openwrt.git --depth 1
cd openwrt

# apply patch
git apply patches/openwrt/21.02.5/0001-add-hatlab-gateboard-one.patch

# install feeds
./scripts/feeds update -a
./scripts/feeds install -a

# make menu config
#   Target System:
#     MediaTek Ralink MIPS
#     MT7621 based board
#     HATLab GateBoard-One
make menuconfig

# make build
make
```
