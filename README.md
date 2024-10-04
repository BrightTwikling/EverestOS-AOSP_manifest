# This is ProjectEverest [EverestOS]
### Initialize local repository
```
repo init -u https://github.com/BrightTwikling/EverestOS-AOSP_manifest -b 15_zf7 --git-lfs
```
### Sync up 
```
repo sync -c --force-sync --optimized-fetch --no-tags --no-clone-bundle --prune -j$(nproc --all)
```
# Build
```
. build/envsetup.sh
```
```
lunch everest_<devicecodename>-ap3a-<build_type>
```
```
make everest -j$(nproc --all)
```
