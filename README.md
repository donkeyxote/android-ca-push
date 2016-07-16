# android-ca-push

Bash script for easy pushing of user-selected certification authority's certificates on android devices.

## HowTo

edit ``cert_list.conf`` and add your favourite certificate urls.

connect your android device and make sure it is correctly recognized by **adb**.

    $ adb devices
    0123456789abcdef        device

launch ``android-ca``

    $ chmod u+x android-ca
    $ ./android-ca install

## Commands

* ``android-ca install`` shortcut for ``android-ca update; android-ca hash; android-ca push; android-ca clean``
* ``android-ca update`` get new certificates.
* ``android-ca hash`` create Android compatible certificate files from the original certificate files.
* ``android-ca push`` push certificates to device.
* ``android-ca clean`` remove downloaded files.
* ``android-ca help`` print usage.
