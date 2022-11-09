# wiki
To quickly look up some things that might be needed at some point in the future:

### VPN
#### configure L2TP VPN with nmcli
use:
```
nmcli c add con-name <name> type vpn vpn-type l2tp vpn.data 'gateway=<host>, ipsec-enabled=yes, ipsec-psk=<key>, password-flags=2, user=<user>'
```
then use
```
nmcli c up <name> --ask
``` 
to establish connection
