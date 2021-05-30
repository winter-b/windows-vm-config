# windows-vm-config

[Everything that you will need](https://wiki.archlinux.org/title/PCI_passthrough_via_OVMF)


# Autoboot setup

store rc.local file under /etc directory

# Mounting VM img files in Linux

1. sudo fdisk -l /var/lib/libvirt/images/win10-clone-clone.img
2. mount -o loop,offset={Secotor Size * Device start byte} /var/lib/libvirt/images/win10-clone-clone.img  /mnt/iso
![image](https://user-images.githubusercontent.com/85021800/120117583-807f1780-c196-11eb-9b1d-ca479fc91ce5.png)
Example: sudo mount -o loop,offset=677380096 /var/lib/libvirt/images/win10-clone-clone.img /mnt/iso
