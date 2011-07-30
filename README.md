DroniX Dev Team's 'cucina'
=========================

**cucina** allows you to create Android splash image (*splash.img*) and *logo.rle* image.
Currently it supports Gnu/Linux. You could try any bash+x86_64 capable OS.

Getting started
---------------
`git clone git@github.com:dronixdevteam/cucina.git`

`git checkout -t origin/develop`

`chmod +x menu`



splash.img
----------

splash.img can be created from .png or .jpg image files. Image file size is your Android screen resolution: i.e. 4Geek Horus is 480x800 pixels. Bulk creation is available.

### Usage
Put images into *images/* folder, then run

`./menu`

Choose menu #1. Follow instructions. Converted images will be into *images/* folder.

Flash one of them using fastboot, according to device's partition table, i.e.:

`# fastboot flash splash splash.img`


logo.rle
--------
logo.rle can be created from .png or .jpg image files. Image file size is your Android screen resolution: i.e. 4Geek Horus is 480x800 pixels. Bulk creation is available.

### Usage
Put images into *images/* folder, then run

`./menu`

Choose menu #2. Follow instructions. Converted images will be into *images/* folder.

Rename .rle file to *logo.rle* and put it in your boot.img

License
=======
DroniX Dev Team's 'cucina' is GPL v3 software