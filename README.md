# SUCKLESS UTILS

## patches

```./patches``` containts all the patches I used to configure dwm and st.

To patch a program:
```
patch -p1 < program-patchname.diff
```

## Customisation
personnal note:

To modify or test the intended configurations, all that is needed is editing the ```config.def.h``` file. 

When done, to apply modifications these commands need to be typed:
```bash
sudo cp config.def.h config.h
```
```bash
sudo make clean insall
```

To restart DWM:
```MOD+CTRL+SHIFT+Q```

## DWM
Any script to be executed at startup can be added to ```~/.dwm/autostart.sh```.

Vanitygaps is installed but not used at all, to use it, decomment lines about gaps in ```config.h```.

## ST

## SLSTATUS
