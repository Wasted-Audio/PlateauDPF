Valley Plateau reverb, wrapped in a plugin for convenience.
Original Valley Plateau "free" distribution: https://github.com/ValleyAudio/ValleyRackFree

uses the Component Library graphics © 2016-2023 VCV, more details here:
https://github.com/VCVRack/Rack/blob/v2/LICENSE.md

On Windows, this repo builds a VST3.
On MacOS, this repo builds a VST3 and an AU.

To use:

```
git clone --recursive https://github.com/rubyswolf/Plateau
cd Plateau/plugins/Plateau
make
```

Plugins will be built in the `bin` directory.

NOTE: On a Mac, you may need to remove the quarantine attribute before installing plugins:

```
cd bin # Or wherever your plugins are located
sudo /usr/sbin/xattr -r -d com.apple.quarantine Plateau.component
sudo /usr/sbin/xattr -r -d com.apple.quarantine Plateau.vst3
```

* Author: rubyswolf
* Mac build: lamech

January, 2025
