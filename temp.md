### ip address show
>*show ip addresses*

### ip address add {ip_address/net_mask} dev {interface}
### ip link set {interface} up
>*set up ip address and activation interface*

### ip address add {ip_address/net_mask} broadcast {broadcast_ip_address} dev {interface}
### ip link set {interface} up
>*set up ip address with broadcvast settings  and activation interface*

### ip route add
>*add route, please see command options for details*

### DNS

### /etc/resolf.conf
>*file with DNS addresses*

### /etc/init.d/network
### etc/init.d/networking

>*system startup network scenario*
>*--start  switch on settings*
>*--stop   switch off settings*

>Interface configuration files, that use /etc/init.d/network(ing), in different Linux versions named differently, according to system, that uses for network configuration, for example in *etcnet* catalogue with settings named as: */etc/net*, and also in */etc/sysconfig/network*.

>*In *ifupdown* use one file for network interfaces and router configuration.


## DHCP

In Linux DHCP process dhcpd deamon, on of files, that he can change - *resolv.conf*, so if in network works DHCP server, network settings: *ip-address, mask, default gateway, domain name, DHCP server address, broadcast ip-address e.t.c*, can be given over dhcpd and Linux will automatically configure network connection.

## PPP

This is moded access.
Deamons:
* pppd

Utilites:
* kppp: /etc/ppp (configuration files)
* wvdial

### PPPoE

Deamons:
* pppd + pppoe (virtual modem interface)

## NETWORK FIREWALL AND NAT

### iptables
>*linux firewall utilite*

### iptables-save
>*list all rules in all tables*


## HTTP BROWSERS AND SERVERS

Apache 
thhtpd
tux module for kernel

## FTP

*  FTP - required for public archives.
* PFTP - Passive FTP through client Firewall.

## TERMINAL ACCESS

* TELNET - telnet, telnetd, not sequre.
* SSH - ssh, sshd.

## E-MAIL
* mail - utilite for mailing.
* sendmail - old SMTP server.
* postfix - SMTP server.
* QMail -   SMTP server.
* Exim - SMTP server.
* ZMailer - for high load servers.

IMAP servers:

* Cyrus
* UW-IMAP
* Binc


