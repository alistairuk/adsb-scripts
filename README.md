# adsb-wiki
Solutions to common problems using dump1090 variants and ADS-B feeders


## Install script for dump1090-fa

- automatically reconfigures fr24feed (if installed)
- fixes read-only problem with pi24 image
- installs dump1090-fa
- makes it possible to change gain without editing a file


### changing gain with provided helper:

(might only work after rebooting after you used the script)

```
sudo dump1090-fa-gain 42.1
```


Available gain settings:
```
0.0 0.9 1.4 2.7 3.7 7.7 8.7 12.5 14.4 15.7 16.6 19.7 20.7 22.9 25.4
28.0 29.7 32.8 33.8 36.4 37.2 38.6 40.2 42.1 43.4 43.9 44.5 48.0 49.6 -10
```
(-10 is a special setting which in practice equals a gain of around 55)
