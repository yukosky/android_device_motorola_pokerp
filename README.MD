# OrangeFox Recovery Project for the Moto E6 Plus

### How to build ###

```bash
# Create dirs
$ mkdir ofox; cd ofox

# Init repo
$ repo init --depth=1 -u https://gitlab.com/OrangeFox/Manifest.git -b fox_9.0

# Clone pokerp repo
$ git clone https://github.com/yukosky/android_device_motorola_pokerp -b fox-9.0 device/motorola/pokerp

# Sync
$ repo sync --no-repo-verify -c --force-sync --no-clone-bundle --no-tags --optimized-fetch --prune -j`nproc`

# Build
$ chmod -R +x device/motorola/pokerp/build_ofox.sh; mv device/motorola/pokerp/build_ofox.sh .
```

## Credits
* Astrako: For build_ofox.sh file
* rssxda: For base device tree
