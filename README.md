# macrogaura - RGB keyboard control for Asus ROG laptops on 

(c) 2021 TSLARoadster

Supports RGB keyboards with IDs
[0b05:1854](https://linux-hardware.org/index.php?id=usb:0b05-1854)
(GL553, GL753),
[0b05:1869](https://linux-hardware.org/index.php?id=usb:0b05-1869)
(GL503, FX503, GL703), [0b05:1866](https://linux-hardware.org/index.php?id=usb:0b05-1866) (GL504, GL703, GX501, GM501), and [0b05:19b6](https://linux-hardware.org/index.php?id=usb:0b05-19b6) (GA503).

## Usage

1. Download latest binary release
2. Extract and put it in `/usr/local/bin`
3. Use with the commands below

```
Usage:
   macrogaura [-v] COMMAND ARGUMENTS

COMMAND should be one of:
   single_static
   single_breathing
   single_colorcycle
   multi_static
   multi_breathing
   red
   green
   blue
   yellow
   gold
   cyan
   magenta
   white
   black
   rainbow
   brightness
   initialize_keyboard
```

If your keyboard does not respond to `macrogaura`, it may help to
send an initialisation message to the keyboard to "wake it up":

```
macrogaura initialize_keyboard
```

*Sometimes root privileges is needed if it doesn't work, in that case use `sudo` before each command*

## Building

Clone the GitHub repo and enter the top-level directory.  Then:

```
sudo xcodebuild
```

## Credits
- [Will Roberts](https://github.com/wroberts) for [rogauracore](https://github.com/wroberts/rogauracore) (based on which this program was developed)
- [Le Bao Hiep](https://github.com/hieplpvip) for porting rogauracore to macOS
- [TSLARoadster](https://github.com/TSLARoadster) for maintaining macrogaura
