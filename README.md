---------------------------------------------------------------------------------------
 Getting Started:
 ==============

To get started with Octavi-OS, you'll need to get familiar with [Repo](https://source.android.com/source/using-repo.html) and Version Control with [Git](https://source.android.com/source/version-control.html).

To initialize your local repository, use a command like this:

```bash
repo init -u https://github.com/OctaviOS-fork/android_manifest.git -b thirteen --git-lfs
```
or
```bash
repo init --depth=1 --no-repo-verify -u https://github.com/OctaviOS-fork/android_manifest.git -b thirteen --git-lfs -g default,-mips,-darwin,-notdefault
```

Then to sync up:

```
repo sync -c -f --force-sync --optimized-fetch --no-tags --no-clone-bundle --prune -j8
```
or
```
repo sync -c --force-sync --optimized-fetch --no-tags --no-clone-bundle --prune --retry-fetches=5 -j$(nproc --all)
```

---------------------------------------------------------------------------------------
 Compilation of OctaviOS:
 ==================

From root directory of Project, perform following commands in terminal

```bash
$ . build/envsetup.sh
$ lunch octavi_$device-userdebug
$ mka bacon -j$(nproc --all)
```

---------------------------------------------------------------------------------------

 More stuff :
 =======================
 
 * [**Bringup Guide for Octavi-OS**](https://github.com/Octavi-OS/Stuff)
 * [**XDA Thread**](https://github.com/Octavi-OS/xda)

---------------------------------------------------------------------------------------

### Links to official groups/channels
- [**Discussion Group**](https://t.me/ArataXDummy)
- [**Announcements Channel**](https://t.me/mirrorlinkbyvinz)
