# linuxBasicForHackers

## Estas son las notas de lo que aprendo del libro " Linux basics for hackers" 


### Analyzing and managing networs

#### Analyzing networks with ifconfig

`ifconfig`    muestra la configuracion de nuestra interface de redes 

`iwconfig`    muestra la configuracion de redes pero en wifi.

`ifconfig eth0 192.168.181.115`     Cambianos nuestra direccion IP. 

`ifconfig eth0 192.168.181.115 netmask 255.255.0.0 broadcast 192.168.1.255`   Cambiamos nuestra mascara de red y el broadcast address. 


#### Spoofing the Mac Address. 

Este es uno de los mas basicos movimientos para evitar se trackeados y tambien para mantener a los hackers fuera de nuestra red.

`ifconfig eth0 down`  primer paso. 
`ifconfig eth0 hw ether 00:11:22:33:44:55`    Cambiamos la direccion Mac. 
`ifconfig eth0 up`      reactivamos la direccion Mac.
