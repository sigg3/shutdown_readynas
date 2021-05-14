# shutdown_readynas
Small utility written in python3 to shutdown a running Netgear ReadyNAS using browser automation.

This utility targets old ReadyNAS units that have the RAIDiator 4.2.31 web interface (on TLS1).

And yes, it is rather overkill. But it does the job.

```
Warning: The ReadyNAS uses a very old self-signed certificate. By default, we
wait to transmit login credentials until after a session has been established,
but there ARE NO GUARANTEES that the GET requests cannot be read on the LAN.

Usage:
    shutdown_readynas [options] <NAS IP address>

Options:
    --user=<string>      To use a different admin user. Default is 'admin'
    --password=<string>  This is bad practice. Omit to use the prompt instead.
```

# TODO
0. Verify that we do not send GET request in the open
1. There are currently 2 known errors to handle: web-server cold boot (timeout) and wrong password.
2. Package it up in __main__, python style.
