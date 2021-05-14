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
VBoxManage.exe modifymedium "C:\Users\Beesion\VirtualBox VMs\Blazedpath\blazedpath\blazedpath-disk1.vdi" -compact
```


# install
- [install](http://informatica.iesvalledeljerteplasencia.es/wordpress/instalacion-de-xubuntu-18-04-lts-en-virtualbox/)  
- [additions](https://www.diversidadyunpocodetodo.com/instalar-guest-additions-ubuntu-compartir-unidades-almacenamiento/)
- [additions-2](https://cambiatealinux.com/instalar-las-guest-additions-virtualbox-ubuntu-server)