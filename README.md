# razerduino

Exploit a privlage escalation bug in razer's synaps installer with an arduino pro micro explained in [this tweet](https://twitter.com/j0nh4t/status/1429049506021138437).
This custom board emulates a "Mamba 2015 Tournament Edition" mouse.

## Installation

1. Open `File -> prefrences` and add [https://raw.githubusercontent.com/DarkMetalMouse/razerduino/master/package_razerduino_index.json](https://raw.githubusercontent.com/DarkMetalMouse/razerduino/master/package_razerduino_index.json) to `Additional Boards Manager URLS`
2. Go to `Tools -> Board: "XYZ" -> Boards Manager...`
3. In the window that pops up, search `razerduino` and click install
4. Once the install is done, select the `Razer Arduino Micro` from `razerduino`
5. Open `File -> Examples -> HID -> EnableMouse` and upload the code

## Customization

If you would like to emulate a different device, change the [build PID inside boards.txt](https://github.com/DarkMetalMouse/razerduino/blob/master/0.9.0/boards.txt#L44) to a PID from [this list](https://the-sz.com/products/usbid/index.php?v=0x1532). It may not work with older products and non mouse devices.
