
## Recovery Device Tree for the Samsung Galaxy M21  (Exynos-9611)
Prebuilt Image with latest official Source Kernel Samsung M21

## Getting Started ##
To get started with AOSP sources to build TWRP, you'll need to get familiar
with [Git and Repo](https://source.android.com/source/using-repo.html).

To initialize your local repository using the AOSP trees to build TWRP, use a command like this:

    repo init -u https://github.com/minimal-manifest-twrp/platform_manifest_twrp_aosp.git -b twrp-12.1

To initialize a shallow clone, which will save even more space, use a command like this:

    repo init --depth=1 -u https://github.com/minimal-manifest-twrp/platform_manifest_twrp_aosp.git -b twrp-12.1

Then to sync up:

    repo sync

## How-to compile it:

```sh
export ALLOW_MISSING_DEPENDENCIES=true;
. build/envsetup.sh;
lunch twrp_m21-eng;
mka recoveryimage
```
