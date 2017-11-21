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

## Licence

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License. You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.
