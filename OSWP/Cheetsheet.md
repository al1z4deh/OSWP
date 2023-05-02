Mueyyen bir chanall-da ise salmaq ucun

```
sudo airmon-ng start wlan0 3
```

Hansi chanall-da oldugumuzu gormek ucun

```
sudo iw dev wlan0mon info
```

Deqiq iyleme

```
sudo airodump-ng -c 3 --bssid 34:08:04:09:3D:38 -w cap1 wlan0mon
```
