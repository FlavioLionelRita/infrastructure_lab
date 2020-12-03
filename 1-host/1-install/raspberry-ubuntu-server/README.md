



# install
```
sudo apt update
sudo apt upgrade
sudo apt-get install tasksel
sudo tasksel
```
select: "ubuntu minimal desktop"

## enable SSH
```
sudo apt install ssh
sudo apt-get install openssh-server
sudo /etc/init.d/ssh start
sudo systemctl enable ssh
```
verify
```
sudo systemctl is-enabled ssh
```

Lionel02

## instal VNC server
```
sudo apt update
sudo apt install xfce4 xfce4-goodies
sudo apt install tightvncserver
vncserver
```
set password: Lionel02

execute
```
vncserver -kill :1
mv ~/.vnc/xstartup ~/.vnc/xstartup.bak
sudo vim ~/.vnc/xstartup
```
add content
```
#!/bin/bash
xrdb $HOME/.Xresources
startxfce4 &
```

execute
```
sudo chmod +x ~/.vnc/xstartup
vncserver 
```


# pendiente habilizar ventilador
sudo apt-get install -y rpi.gpio-common
gpio write 17 0
gpio export 17 out
echo "1" > /sys/class/gpio/gpio17/value
sudo echo 17 > /sys/class/gpio/export
sudo echo out > /sys/class/gpio/gpio17/direction
sudo echo 1 > /sys/class/gpio/gpio17/value
https://zoomadmin.com/HowToInstall/UbuntuPackage/rpi.gpio-common



# Acceder desde windows a las otras maquinas por SSH

# On server linux
## enable SSH
```
sudo apt install ssh
sudo apt-get install openssh-server
sudo /etc/init.d/ssh start
sudo systemctl enable sshd
```
verify
```
sudo systemctl is-enabled sshd
```


https://www.cyberciti.biz/faq/linux-start-sshd-openssh-server-command/
https://www.redeszone.net/gnu-linux/servidor-ssh-en-ubuntu/
https://www.sololinux.es/habilitar-el-servicio-ssh-en-ubuntu-20-04/


# On Host Windows

## install NMAP
namp es un programa para escanear las maquinas que estan conectadas en la red.
descargar he instalar: [download](https://nmap.org/book/inst-windows.html)

## net scanner 
```
nmap 192.168.1.0/24
```
## install mRemoteNG




# references
## install
- [install] (https://ubuntu.com/tutorials/how-to-install-ubuntu-on-your-raspberry-pi#1-overview)
- [install video](https://www.youtube.com/watch?v=fjb7pD5GYDo)
- [install ubuntu on raspberry](https://ubuntu.com/download/raspberry-pi)
##  vnc server
- [install vnc-server](https://www.digitalocean.com/community/tutorials/how-to-install-and-configure-vnc-on-ubuntu-20-04-es) 
## others
- [automatizar ventilador](https://www.raspberrypi.org/forums/viewtopic.php?p=534742#p534742)
- [pines raspberry](https://elinux.org/RPi_Low-level_peripherals#General_Purpose_Input.2FOutput_.28GPIO.29)






