# Ilvaite &nbsp; [![bluebuild build badge](https://github.com/luciofstars/ilvaite/actions/workflows/build.yml/badge.svg)](https://github.com/luciofstars/ilvaite/actions/workflows/build.yml)

Ilvaite is an opinionated, low-fat atomic distribution built from Universal Blue and Fedora Atomic. It's primarily intended for my personal use, with the applications I depend on pre-installed and ready to use. **If you're looking to make your own personal image, you're better off starting from the upstream [BlueBuild sources](https://blue-build.org/).**

# Installation
These installation steps have only been tested from a clean installation of Fedora Kinoite.

- First, rebase to the unsigned image to get the proper signing keys and policies installed:
  ```
  rpm-ostree rebase ostree-unverified-registry:ghcr.io/luciofstars/ilvaite:latest
  ```
- Reboot your system, then rebase to the signed image, like so:
  ```
  rpm-ostree rebase ostree-image-signed:docker://ghcr.io/luciofstars/ilvaite:latest
  ```
- Reboot again to boot the signed image. You're done!

# Contributions
Contributions are welcomed, but may not be accepted. If it doesn't improve my personal system in a meaningful way, it probably won't be merged. Anything that makes it easier to install/re-install/build is fine.

# License
Ilvaite's build scripts (this repository) are free as in freedom. You can redistribute them and/or modify them under the terms of the **GNU General Public License** as published by the Free Software Foundation; either version 3 of the License, or (at your option) any later version.

The software that comprises the Ilvaite distribution is released under a myriad of different licenses. See the Fedora Project and Universal Blue for more information, or contact the author(s) of the software.