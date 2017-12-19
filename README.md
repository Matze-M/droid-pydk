# droid-pydk


# An android python framework assistant. 


While helping to cross-compile, the script also try to prepare a onboard sdk (armv7 currently).

Requirements : GNU/Linux os , NDK 14b and SDK


Usage for cross compile i like "/data/data" path so it matches devices layout :
--

```
sudo mkdir /data

sudo chown $(whoami) /data

bash ./frankenbuild.sh /data/data 192.168.0.xxx*
```

*The ip addr is for targeting an adb networked device such as an h3droid board no IP means use classic adb over usb.


after install you can parse . /data/data/sdk.env to enter the build zone where you'll find various .build file which are recipe to download / patch / build for your presets.
