# ckb-next-ubuntu
Rough and ready debian package scripts for [ckb-next](https://github.com/mattanger/ckb-next) the open source Corsair Keyboard and Mouse RGB Driver for Linux and OS X.

## Pre-built packages
You can find pre-built packages on the [releases page](https://github.com/dameikle/ckb-next-ubuntu/releases) that can be downloaded and installed on your system.

The packages are all signed with my [public key](https://keyserver.ubuntu.com/pks/lookup?op=get&fingerprint=on&search=0xA9BD932BAF95099A) and you can verify them using

    gpg --verify <filename>.dsc
  
## Building your own package
Having clones this repository, you can build your own deb package using the following command:

    dpkg-buildpackage -us -uc -b

This will create an unsigned, binary only package that is ideal for your own use.

## Dependencies

Ensure you have those packages installed if you want to build your own packages:

 - `build-essential`
 - `debhelper`
 - `pkg-create-dbgsym` (optional, only for Ubuntu systems)
