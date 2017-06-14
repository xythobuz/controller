# Quick Start

My KLL files (generated with the Input Club Configurator) are stored in this repository. Checkout the proper kll version (master will be checked out automatically on build, probably too new):

    cd kll
    git checkout 2062be08e34430d523b20947e9eb5a3ec3948331

Then copy the custom kll files into `kll/layouts/`. Now, run the build process:

    cd Keyboards
    ./my_ergodox.bash

Then update the firmware:

    sleep 5 && dfu-util -D right_kiibohd.dfu.bin
    (Quickly enable flash-mode (Layer 2, ‘=‘ button))

For simple layout changes flashing the right half is enough. Deeper firmware changes probably require flashing both halves separately.

