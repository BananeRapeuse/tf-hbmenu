### Usage
See [Homebrew_Applications](https://switchbrew.org/wiki/Homebrew_Applications) for SD layout and applications, etc. See [Switchbrew](https://switchbrew.org/wiki/Homebrew_Menu) for hbmenu docs.

### Download
The latest release is available from the [releases](https://github.com/BananeRapeuse//tf-homebrew-launcher/releases/) page.

### Building
Build for the Nintendo Switch with ```make nx``` and for the PC with ```make pc```.
Running ```make``` builds for both systems.

The following [pacman packages](https://devkitpro.org/wiki/devkitPro_pacman) are required to build for Switch:
- `switch-dev`
- `switch-freetype`
- `switch-libconfig`
- `switch-libjpeg-turbo`
- `switch-physfs`

The following libraries are required to build for PC:
- `libfreetype`
- `libconfig`
- `libjpeg-turbo`
- `libphysfs`

Building for Switch/PC requires `zip`.

Since C11 threads are used, building for the PC may fail if C11 threads are not available.

#### Credits

* This uses code based on 3DS [new-hbmenu](https://github.com/fincs/new-hbmenu).
* `libjpeg-turbo` is used for handling JPEG icons. This library doesn't support lossless JPEG (likewise for official sw which uses `libjpeg-turbo`).
* Special thanks for [PoloNX](https://github.com/PoloNX) for the help to compile the program with devkitPro. 
