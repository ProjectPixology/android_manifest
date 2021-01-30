Welcome to pixology.
===========

Installation
---------------

To get started with the installation, you'll need to get
familiar with [Repo](https://source.android.com/source/using-repo.html) & [Version Control with Git](https://source.android.com/source/version-control.html).

To install the sources onto your system, you will need to first run
```bash
repo init -u git://github.com/ProjectPixology/android_manifest.git -b eleven
```
Then to sync up:
```bash
repo sync --force-sync --no-tags --no-clone-bundle -j$(nproc --all)
```
Build
---------------
```bash
. build/envsetup.sh
lunch lineage_device-userdebug
mka bacon -j4
```
