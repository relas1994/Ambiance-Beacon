For Prototype.c and Server.c the folling libraries versions are used:
wiringPi version: 2.32
libqrencoede version: 3.9.0
MYSQL version: 5.5.44- 0+deb8u1
gcc version: 4.9.2
Raspbian version: 4.9.2-10
Apache server version: 2.4.10
PHP version:  5.6.20-0+deb8u1

commando's for the initialisation of the programmas
Prototype: gcc -o Prototype $(mysql_config --cflags) Prototype.c $(mysql_config --libs) -lwiringPi
Server:gcc -o Server$(mysql_config --cflags) Server.c $(mysql_config --libs)

Commando for generating the QR code
qrencode -o local.png (IP-adres)

location for the local.png file
/var/ww/html

