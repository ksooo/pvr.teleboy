# Teleboy PVR addon for Kodi

This is a [Kodi](https://kodi.tv) PVR addon for streaming live TV from [Teleboy](https://www.teleboy.ch).

## Build instructions

1. `git clone --branch master https://github.com/xbmc/xbmc`
2. `git clone --branch Matrix https://github.com/rbuehlma/pvr.teleboy`
3. `cd pvr.teleboy && mkdir build && cd build`
4. `cmake -DADDONS_TO_BUILD=pvr.teleboy -DADDON_SRC_PREFIX=../.. -DCMAKE_BUILD_TYPE=Debug -DCMAKE_INSTALL_PREFIX=../../xbmc/addons -DPACKAGE_ZIP=1 ../../xbmc/cmake/addons`
5. `make package-pvr.teleboy`