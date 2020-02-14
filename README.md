# Home-Assistant


open SD

/etc/wpa_supplicant/wpa_supplicant.conf 

```
ctrl_interface=DIR=/var/run/wpa_supplicant GROUP=netdev
update_config=1
country=CN
network={
	ssid=""
	scan_ssid=1
	psk=""
}
```

/etc/apt/sources.list
```
deb http://mirrors.tuna.tsinghua.edu.cn/raspbian/raspbian/ buster main non-free contrib
deb-src http://mirrors.tuna.tsinghua.edu.cn/raspbian/raspbian/ buster main non-free contrib
```

```
sudo apt update
sudo apt install python3
sudo apt install python3-dev
sudo apt install python3-setuptools
sudo apt install python3-pip
sudo apt install libffi-dev
```

~/.pip/pip.conf
```
[global] 
index-url = https://pypi.tuna.tsinghua.edu.cn/simple
[install]
trusted-host = https://pypi.tuna.tsinghua.edu.cn
```

```
pip3 install PyQRCode
pip3 install defusedxml
pip3 install distro
pip3 install aiohttp_cors
pip3 install homeassistant
hass --open-ui
```

/etc/rc.local
```
su pi -c "exec /home/pi/hass.sh"
```

hass.sh
```
hass
```

然后打开浏览器，浏览：http://localhost:8123

android手机可以使用：https://github.com/tuanha2000vn/hasskit/releases/download/4.3/app-release.apk

ios的在appstore里搜索hasskit即可。


