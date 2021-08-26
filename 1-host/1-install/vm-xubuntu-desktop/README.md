# Vitual machine data
- so: xubuntu 18.04
- user: flavio
- password: flavio


# additions
```
sudo apt-get update
sudo apt-get upgrade
sudo apt-get install virtualbox-guest-additions-iso
```


# liberar espacio en Virtual Box
Liberar espacio en VM

## En maquina virtual
	sudo dd if=/dev/zero of=zerofillfile bs=1M
	sudo rm zerofillfile
## En el Host
```
cd C:/Program Files/Oracle/VirtualBox
VBoxManage.exe modifymedium "C:\vm\20210826\20210826-disk1.vdi -compact
```
# Aumentar espacio en Virtual Box
```
cd C:/Program Files/Oracle/VirtualBox
VBoxManage modifyhd "C:\vm\20210826\20210826-disk1.vdi" --resize 65536
```



# install
- [install](http://informatica.iesvalledeljerteplasencia.es/wordpress/instalacion-de-xubuntu-18-04-lts-en-virtualbox/)  
- [additions](https://www.diversidadyunpocodetodo.com/instalar-guest-additions-ubuntu-compartir-unidades-almacenamiento/)
- [additions-2](https://cambiatealinux.com/instalar-las-guest-additions-virtualbox-ubuntu-server)
- [aumentar disco](https://duenaslerin.com/aumentar-tamano-disco-virtual-virtualbox/)
