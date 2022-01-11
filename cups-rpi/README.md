# Home Assistant Add-on: CUPS Raspberry Pi

# Add printers to the Cups server
Connect to the Cups server at http://127.0.0.1:631

Add printers: Administration > Printers > Add Printer
Note: The admin user/password for the Cups server is print/print

# Configure Cups client on your machine
Install the cups-client package
Edit the /etc/cups/client.conf, set ServerName to 127.0.0.1:631
Test the connectivity with the Cups server using lpstat -r
Test that printers are detected using lpstat -v
Applications on your machine should now detect the printers!

# Included package
cups, cups-client, cups-filters
foomatic-db
printer-driver-all, printer-driver-cups-pdf
openprinting-ppds
hpijs-ppds, hp-ppd
sudo, whois
smbclient

![Supports armhf Architecture][armhf-shield]
![Supports armv7 Architecture][armv7-shield]

[armhf-shield]: https://img.shields.io/badge/armhf-yes-green.svg
[armv7-shield]: https://img.shields.io/badge/armv7-yes-green.svg
