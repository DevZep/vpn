# DevZep VPN

## Installation

Follow the instructions [here](https://www.cyberciti.biz/faq/howto-setup-openvpn-server-on-ubuntu-linux-14-04-or-16-04-lts/).

## Configuring DevZep VPN

Follow the instructions [here](https://www.cyberciti.biz/faq/howto-setup-openvpn-server-on-ubuntu-linux-14-04-or-16-04-lts/).

## Creating new Clients

Log into the VPN server and run:

```
sudo bash openvpn-ubuntu-install.sh
```

You will be presented with the following menu:

```
OpenVPN is already installed.

Select an option:
   1) Add a new client
   2) Revoke an existing client
   3) Remove OpenVPN
   4) Exit
```

Type 1 and you will see:

```
Provide a name for the client:
Name:
```

Type in a suitable name and press enter.

Now use scp to copy the generated `.ovpn` file to your machine and then copy onto the client device.

If using [Tunnelblick](https://tunnelblick.net/) then you can drag the config into the Tunnelblick window to add that config to your client. Then connect and you are now using the DevZep VPN!