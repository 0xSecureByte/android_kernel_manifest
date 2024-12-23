
## Repo Init ##
```bash
repo init -u https://github.com/0xSecureByte/android_kernel_manifest.git -b android-msm-lunaa-5.4-android13
```
## Sync Source ##
```bash
repo sync --force-sync --no-clone-bundle --current-branch --no-tags -j$(nproc --all)
```
## Build ##
For Clang builds
```bash
BUILD_CONFIG=kernel/msm-5.4/build.config.msm.lahaina VARIANT=qgki LTO=full BUILD_KERNEL=1 build/build.sh
```
