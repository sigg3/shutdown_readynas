# shutdown_readynas
Small utility written in python3 to shutdown a running Netgear ReadyNAS using browser automation.

This utility targets old ReadyNAS units that have the RAIDiator 4.2.31 web interface (on TLS1).

Yes, it is rather overkill, but it works.

Usage: ./shutdown_readynas &lt;IP> &lt;PASSWORD>

# TODO
0. Change to ./shutdown_nas &lt;IP> and prompt for password
1. Or allow separate --password argument (unsafe)
2. Ping before prompting
3. Allow --noping in case of IGMP block
4. There are currently 2 known errors to handle: web-server cold boot (timeout) and wrong password. (Successful execution shows "Done.")
