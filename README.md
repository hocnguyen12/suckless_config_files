# Suckless utils

see https://suckless.org/

![screenshot](./screenshots/2024-01-14-225548_1366x768_scrot.png)

## patches

```./patches``` containts all the patches used to configure dwm and st.

Patching:
```
patch -p1 < program-patchname.diff
```

## Customisation
note:

To modify or test the intended configurations, all that is needed is editing the ```config.def.h``` file. 

When done, to apply modifications use these commands:
```bash
sudo cp config.def.h config.h
```
```bash
sudo make clean insall
```

To restart DWM: (restartsig)
```MOD+CTRL+SHIFT+Q```

## dwm
MOD/SUPER key is bound to the Windows key aka ```Mod4Mask```.

Any script to be executed at startup can be added to ```~/.dwm/autostart.sh```.

To bind volume keys, added the alsa volume commands bound with ```XF86keysym```.

## st

Colorscheme: color themes can be added or edited in ```config.h``` the ```static const ColorScheme scemes[]```. 

Fonts can be downloaded and moved to a ```~/.fonts``` directory and edited in ```config.h```.

## slstatus

Displaying sound volume is displayed via a script/command.

Downloaded the ```alsa-utils``` package and edited dwm config to bind sound keys.

## void-src packages
In ```~/.local/share/pkgs``` (created pkgs directory), clone the ```void-packages``` repository.

```bash
$ git clone https://github.com/void-linux/void-packages.git
```
then follow the quickstart instructions.
