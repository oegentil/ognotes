# ifconfig to ip equivalent commands #

ifconfig | ip
---|---
$ ifconfig | ip
$ ifconfig -a | ip
$ ifconfig -s | ip
$ ifconfig -v | ip
$ ifconfig &lt;INTERFACE&gt; | ip
$ ifconfig eth0 up | ip
$ ifup eth0 | ip
$ ifconfig eth0 down | ip
$ ifdown eth0 | ip
$ ifconfig | grep inet | ip
$ ifconfig | grep -w inet | ip
$ sudo ifconfig eth0 198.12.14.123 | ip
$ ifconfig | grep netmask | ip
$ sudo ifconfig eth0 netmask 255.255.255.250 | ip
$ ifconfig | grep broadcast | ip
$ sudo eth0 broadcast 192.162.125.200 | ip
$ sudo ifconfig eth0 198.12.14.123 netmask 255.255.255.200 broadcast 192.162.125.200 | ip
$ ifconfig | grep mtu | ip
$ sudo ifconfig eth0 mtu 1000 | ip
$ sudo ifconfig eth0 promisc | ip
$ sudo ifconfig eth0 -promisc | ip
$ sudo ifconfig eth0:0 198.12.14.123 | ip
$ ifconfig eth0:0 | ip
$ ifconfig eth0:0 down | ip
$ ifconfig | grep ether | ip
$ sudo ifconfig eth0 down | ip
$ sudo ifconfig eth0 hw ether AA:BB:CC:DD:EE:FF | ip
$ sudo ifconfig eth0 up | ip
$ sudo eth0 arp | ip
$ sudo eth0 -arp | ip
$ sudo ifconfig eth0 allmulti | ip
$ sudo ifconfig eth0 -allmulti | ip
$ sudo ifconfig eth0 add 2001:0db8:0:f101::1/64 | ip
$ sudo ifconfig eth0 del 2001:0db8:0:f101::1/64 | ip
$ sudo ifconfig eth0 trailers | ip
$ sudo ifconfig eth0 -trailers | ip
$ sudo ifconfig sl0 172.16.62.1 point-to-point 172.16.62.2 | ip
$ sudo ifconfig sl0 172.16.62.1 -point-to-point 172.16.62.2 | ip
$ sudo ifconfig sit0 up | ip
$ sudo route -A inet6 add 2000::/3 gw ::192.88.99.1 dev sit0 | ip
$ sudo route -A inet6 del 2000::/3 gw ::192.88.99.1 dev sit0 | ip
$ sudo ifconfig sit0 del 2002:80b0:b807::1/16 | ip
$ sudo ifconfig sit0 down | ip
$ sudo ifconfig eth0 txqueuelen 5000 | ip
/sbin/ifconfig eth0 txqueuelen 5000 | ip
$ ifconfig | grep errors | ip
$ curl ifconfig.me | ip
$ ifconfig --help 5 | ip


ref: https://access.redhat.com/sites/default/files/attachments/rh_ip_command_cheatsheet_1214_jcs_print.pdf

ref: https://www.cyberciti.biz/faq/linux-ip-command-examples-usage-syntax/
