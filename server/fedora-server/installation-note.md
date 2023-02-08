https://docs.fedoraproject.org/pt_BR/fedora-server/installation/
https://www.youtube.com/watch?v=FxWinfw-HpI
# requirements
### minimum requirement
- storage space min 5 GiB ::: installed system occupies 2.5 GiB
- memory min 1 GiB 




::::
; changing the resolution
vim /etc/default/grub
add => 
GRUB_CMDLINE_LINUX_DEFAULT="nomodeset"
GRUB_GFXPAYLOAD_LINUX=1280-720
then => run grub2-mkconfig => reboot

; configuring static ip NETWORKING
nmcli connection(or con) modify(or mod) enp0s3 ipv4.address vbox ipv4 address 
ipv4.gateway 10.0.2.1 (example) ipv4.dns 10.0.2.1 (same as gateway) 
ipv4.method manual

nmcli con down enp0s3
nmcli con up enp0s3
;;; ssh connection
https://medium.com/codemonday/ssh-to-virtualbox-port-forwarding-from-wsl2-machine-1f667da18430

;;; connecting to ur vbox linux vm using ssh and port forwarding 
https://www.youtube.com/watch?v=Kq_JOGX0MW4 
ssh -p PORT(ex:2222) linux_user@localhost (localhost can be 127.0.0.1)

