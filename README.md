# shutdown_readynas
Small utility written in python3 to shutdown a running Netgear ReadyNAS using browser automation.

This utility targets old ReadyNAS units that have the RAIDiator 4.2.31 web interface (on TLS1).

Yes, it is rather overkill, but it works.

Usage: ./shutdown_readynas &lt;IP> &lt;PASSWORD>

# TODO
0. Ping NAS first (connection issues)
1. Test that we're actually on the login page (error handling)
