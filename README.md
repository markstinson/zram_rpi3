# rpi_zram
script to enable zram for raspberry pi

Download the script and copy to /usr/bin/ folder
```
sudo wget -O /usr/bin/zram.sh https://raw.githubusercontent.com/ric96/zram_rpi3/master/zram.sh
```

make file executable
```
sudo chmod +x /usr/bin/zram.sh
```

edit /etc/rc.local file to run script on boot
```
sudo nano /etc/rc.local
```

add line before exit 0
```
/usr/bin/zram.sh &
```
